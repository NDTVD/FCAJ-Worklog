---
title: "Week 9 Worklog"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

**Module 9** — Security, Identity Management (IAM), and Application Hardening

### Week 9 Objectives

- Implement the Principle of Least Privilege using AWS Identity and Access Management (IAM): Users, Groups, Roles, and Policies.
- Understand multi-tier cloud defenses: cryptographic encryption via AWS KMS, credentials isolation in AWS Secrets Manager, and AWS WAF filtering.
- Directly implement practical application security: strict cross-origin policies (CORS) and message rate limiting against chat spam.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **AWS IAM Identity Architecture & Least Privilege Enforcement**<ul><li>Surveyed core IAM constructs: IAM Users, IAM Groups, declarative JSON IAM Policies, and temporary IAM Roles.</li><li>Enforced the Principle of Least Privilege: granting strictly bounded permissions necessary for service roles while locking down AWS root accounts.</li></ul> | Nov 09, 2026 | Nov 09, 2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Security on AWS<br>02 — Preventing Unauthorized Access |
| Tuesday | **IAM Roles for AWS Compute & GitHub Actions OIDC Trust**<ul><li>Analyzed IAM Roles for ECS Tasks: leveraging AWS Security Token Service (STS) to vend short-lived credentials directly to containers, eliminating static access keys.</li><li>Configured GitHub Actions OIDC federation: enabling passwordless CI/CD runners to authenticate directly with AWS via OpenID Connect to deploy frontend code securely.</li></ul> | Nov 10, 2026 | Nov 10, 2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Protecting Networks and Applications |
| Wednesday | **AWS KMS Cryptography & Secrets Manager Storage**<ul><li>Investigated AWS Key Management Service (KMS): managing cryptographic master keys for encryption at rest across Amazon S3, EBS volumes, and RDS databases.</li><li>Explored AWS Secrets Manager: isolating PostgreSQL connection strings and JWT authentication secrets from source code with automated credential rotation.</li></ul> | Nov 11, 2026 | Nov 11, 2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Protecting Data |
| Thursday | **AWS WAF Perimeter Security & Backend CORS Hardening**<ul><li>Analyzed AWS Web Application Firewall (WAF): blocking OWASP Top 10 vulnerabilities (SQLi, XSS) and rate-limiting abusive IP addresses at CloudFront and ALB boundaries.</li><li>Directly configured production CORS policies in `Program.cs`: restricting allowed origins exclusively to Tindy's CloudFront distribution domain and enabling required HTTP verbs.</li></ul> | Nov 12, 2026 | Nov 12, 2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Detecting and Responding to Security Incidents |
| Friday | **Real-Time Message Rate Limiting & Anti-Spam Throttling**<ul><li>Analyzed denial-of-service vulnerabilities in live chat rooms: rapid message flooding overflowing WebSocket memory buffers and degrading client rendering performance.</li><li>Implemented message rate limiting algorithms: restricting user dispatch frequencies to a defined window (e.g., maximum 5 messages per second) with informative client feedback.</li></ul> | Nov 13, 2026 | Nov 13, 2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Additional Security Resources |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

Week 9 provided an opportunity for significant direct technical contributions to the Tindy application codebase. While developing our real-time project messaging system, I recognized that malicious clients could flood chat channels with scripted messages, causing browser rendering lag and backend resource exhaustion.

I implemented message rate limiting and throttling logic. When rapid message bursts are detected, the system smoothly throttles dispatch and presents a clear, polite countdown warning in the React chat UI. Additionally, hardening CORS policies in backend `Program.cs` ensured our APIs exclusively accept requests from our verified CloudFront domain.

### Week 9 Learning Outcomes

- Least privilege permissions and IAM Roles for compute represent foundational cloud security pillars eliminating static credential risks.
- Effective web security combines perimeter defense (AWS WAF), origin boundaries (CORS), and application-level controls (Rate Limiting).
- Application in Tindy: Hardened CORS policies in backend Program.cs; implemented message rate limiting in the chat service to prevent message spam.
