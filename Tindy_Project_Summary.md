# Tindy — AI-Powered Community & Project Matching Platform
**First Cloud AI Journey (FCAJ) Community**

---

## 1. Problem Statement

In technology student communities such as the First Cloud AI Journey (FCAJ), project collaboration and team formation face critical recurring challenges:

1. **Hesitation in Cold Outreach & Introversion:** Students who are newly enrolled or naturally introverted often feel uncomfortable messaging strangers directly on social channels (*"Can I join your team?"*). Consequently, capable individuals miss out on valuable practical experience simply because they hesitate to initiate conversations.
2. **Imbalanced Team Skillsets:** Student teams are typically assembled from existing circles of friends, leading to redundant skillsets while lacking vital specialized roles. A team often possesses multiple backend developers or UI designers but lacks an AI/ML engineer or a Cloud/DevOps specialist to deploy and scale the system.
3. **Fragmented and Unverified Profiles:** Evidence of student competence is scattered across disconnected platforms (GitHub repositories, LinkedIn profiles, certification badges, personal portfolio sites, and static PDF resumes). Project leaders waste substantial time manually verifying whether an applicant's skillset matches project demands.
4. **Disjointed Communication & Lost Context:** Switching among third-party messaging applications (Facebook Messenger, Discord, Telegram, Zalo) fractures the collaboration experience. Recruitment context, candidate statuses, and pending commitments frequently get lost across disparate chat logs.
5. **Limitations of Traditional Keyword Filtering:** Basic keyword search fails to capture semantic alignment between project requirements (e.g., *"Experience building RAG systems and LLM applications"*) and a student's project description (e.g., *"Constructed an enterprise conversational assistant using Amazon Bedrock and PostgreSQL pgvector"*).

---

## 2. Proposed Solution

Tindy provides a centralized, AI-driven platform for project discovery and teammate matching within the FCAJ Community. Unlike superficial user-to-user swiping applications, Tindy centers all interactions on **Projects and Open Positions**, fostering a professional and merit-based environment.

### Key Pillars of the Solution:
- **Centralized FCAJ Student Profile:** Students consolidate technical skills, preferred roles (Frontend, Backend, AI/ML, Cloud), weekly commitment availability, portfolio links, and verified AWS certificates in one unified profile.
- **AI Matching Engine (Deterministic Rules + Semantic Similarity):** Evaluates candidate compatibility against project position criteria using a transparent four-factor weighted formula combined with vector embeddings:
  - Required Technical Skills: 40%
  - Preferred Role Alignment: 30%
  - Weekly Availability Commitment: 20%
  - Optional / Bonus Skills: 10%
- **AI Explain Match:** Rather than displaying an arbitrary percentage, the system explains *why* a project or candidate matches, highlighting **Strong Matches** (matching skills, role alignment) and identifying constructive **Skill Gaps** (skills to learn).
- **Interactive Project Discovery:** Students explore recommended projects through intuitive card actions: **Interested** (apply to position), **Skip** (pass), or **Save for Later**.
- **Integrated Real-Time Communication:** Direct messaging and project workspace chat powered by WebSockets (SignalR) allow candidates and leaders to collaborate immediately within the platform.
- **Enterprise-Grade Cloud Architecture:** Built on AWS (`us-east-1`) with a single-domain entry point via Amazon CloudFront, containerized ASP.NET Core API on Amazon ECS Fargate, Amazon RDS PostgreSQL 17, and Amazon Bedrock for generative AI capabilities.

---

## 3. End-to-End Workflow

The complete end-to-end lifecycle consists of five interconnected stages:

```text
[Stage 1: Profile & Project Initiation]
  Student completes profile & uploads resume (PDF)
  --> GuardDuty scans malware --> Bedrock extracts structured skills & bio draft
  --> Student reviews, edits, and saves profile to RDS PostgreSQL.
  Project Lead publishes Project Opportunity with JD and open position requirements.
                            ↓
[Stage 2: Intelligent Matching & Recommendation]
  Matching Engine calculates weighted compatibility scores & semantic embeddings.
  Student accesses "Explore Projects" --> views curated recommendations with Match Scores.
  Student clicks "Why this project?" to inspect AI Explain Match breakdown.
                            ↓
[Stage 3: Expression of Interest (Application)]
  Student selects a position and clicks "Interested".
  Application transitions to "Pending" status.
  Project Lead receives in-app notification of incoming interested candidate.
                            ↓
[Stage 4: Leader Evaluation & Real-Time Interaction]
  Project Lead inspects candidate's profile, skill tags, and match analysis.
  Lead initiates internal real-time chat via SignalR WebSocket for screening.
  Backend rate limiting safeguards chat against spamming.
                            ↓
[Stage 5: Finalization & Team Capacity Sync]
  Project Lead clicks "Accept" (or "Decline").
  System verifies remaining position capacity and creates formal Team Membership.
  Position filled-seat counter increments (e.g., 0/1 -> 1/1).
  State persistently synchronizes across client UI and PostgreSQL database.
```

---

## 4. Additional Capabilities (Optional & Advanced Features)

1. **Asynchronous PDF Malware Protection:** All uploaded resumes and certificate PDFs are stored in an isolated private S3 Media bucket. AWS GuardDuty Malware Protection scans the file, and EventBridge dispatches verdicts to an Amazon SQS queue. A dedicated background worker validates the file status before any AI model or user is permitted to process or view the document.
2. **Dual-Mode CloudFront Edge Routing:** CloudFront operates as the single reverse proxy for the platform:
   - Dynamic switching between `maintenance` mode (serving static maintenance pages directly from S3) and `live` mode (routing `/api/*` to the internal ALB via CloudFront VPC Origins).
   - WebSocket protocol upgrade (`HTTP 101 Switching Protocols`) over CloudFront for real-time SignalR chat without exposing backend ports publicly.
3. **Backend Request Throttling & Rate Limiting:** Built-in middleware limits message throughput per user session, defending the containerized API and SignalR hub against flooding attacks, preserving ECS container responsiveness, and protecting Bedrock token consumption budgets.
4. **Resilient Disaster Recovery & Rollback Strategy:** Automated database snapshot management paired with EF Core database migration tasks allows the platform to recover from schema drift or rollback releases with verified data consistency.
5. **Future Roadmap Extensions:**
   - *AI Team Builder:* Automated recommendations suggesting complementary teammate combinations to fulfill an entire project roster.
   - *AI Learning Roadmap:* Generative tailored learning milestones for students based on skill gaps detected during application attempts.
   - *Automated GitHub Verification:* Deep analysis of student GitHub repositories to validate claimed technical skills against real commit histories.

---

## 5. Cost Estimation

The infrastructure is budgeted using the **AWS Pricing Calculator** for Region **US East (N. Virginia, `us-east-1`)**, specifically optimized for student and startup demo environments:

| AWS Service Component | Configuration & Sizing Details | Monthly Cost (USD) |
| :--- | :--- | :---: |
| **AWS Fargate (Backend API)** | 1 Linux/x86 Task (0.5 vCPU, 2 GiB RAM) running 730 hours/month | $21.26 |
| **Internal Application Load Balancer** | 1 Internal ALB connected to CloudFront VPC Origin (730 hours) | $16.43 |
| **Amazon RDS for PostgreSQL** | Instance `db.t4g.micro` Single-AZ ($11.68) + 20 GiB gp3 Storage ($2.30) | $13.98 |
| **Public IPv4 Address** | 1 public IPv4 allocation for Fargate task (730 hours) | $3.65 |
| **Amazon CloudFront & Amazon S3** | Static website hosting, media bucket, global edge delivery, OAC | ~$1.00 (pay-as-you-go) |
| **Amazon Bedrock, Secrets Manager, CloudWatch** | On-demand resume extraction, 4 active secrets, centralized logs | ~$1.80 (pay-as-you-go) |
| **TOTAL MONTHLY BASELINE (Always-On)** | **Continuous execution across 730 hours/month** | **~$55.32 – $58.12 / month** |

### Cost Optimization Practices Implemented:
- **Scheduled Demo Strategy:** For evaluation cycles, running Fargate tasks and RDS instances only during active demonstration sessions reduces actual compute spend to **under $15.00 USD total**.
- **Automated Teardown (Workshop 5.7):** Six CloudFormation cleanup templates allow comprehensive resource deletion (DELETE_COMPLETE) within minutes after demonstrations to prevent lingering idle charges.
- **Budget Alerts:** Proactive AWS Budgets alarms configured at $30 and $50 monthly thresholds notify the team via Amazon SNS.
