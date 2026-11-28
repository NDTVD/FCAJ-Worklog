---
title: "Week 13 Worklog"
date: 2024-01-01
weight: 13
chapter: false
pre: " <b> 1.13. </b> "
---

**Module 13** — AWS Well-Architected Framework and Internship Wrap-Up

### Week 13 Objectives

- Master the six foundational pillars of the AWS Well-Architected Framework: Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization, and Sustainability.
- Utilize the AWS Well-Architected Tool to review architectural trade-offs, identify high-risk issues, and document continuous remediation plans.
- Consolidate comprehensive internship milestones, verify end-to-end demo video assets, and finalize the complete bilingual internship report.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Holistic Architecture Review of the Tindy Platform**<ul><li>Deconstructed the complete Tindy cloud topology: analyzing the decoupled static CloudFront layer, public ALB routing tier, containerized ECS Fargate compute layer, managed RDS PostgreSQL database, and S3 asset buckets.</li><li>Assessed failure isolation and single-point-of-failure risks across each architectural boundary, establishing baseline performance metrics for concurrent user traffic.</li></ul> | Dec 07, 2026 | Dec 07, 2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Well-Architected Solutions |
| Tuesday | **Exploration of AWS Specialized Services**<ul><li>Explored specialized enterprise services: AWS X-Ray for distributed request tracing, AWS AppSync for real-time GraphQL subscriptions, and AWS Amplify for rapid full-stack scaffolding.</li><li>Contrasted Amazon SES for transactional notification emails and Amazon Connect for cloud contact centers against our current decoupled communication architecture.</li></ul> | Dec 08, 2026 | Dec 08, 2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — AWS Specialized Services |
| Wednesday | **The Six AWS Well-Architected Framework Pillars**<ul><li>Deep dive into the 6 pillars: Operational Excellence (CI/CD release automation), Security (IAM boundaries, KMS, CORS), Reliability (Multi-AZ, health checks), Performance Efficiency (CloudFront CDN caching), Cost Optimization (Fargate serverless, S3 lifecycle), and Sustainability.</li><li>Conducted a structured review within the AWS Well-Architected Tool, evaluating workload risks and documenting strategic architectural trade-offs.</li></ul> | Dec 09, 2026 | Dec 09, 2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — AWS Well-Architected Framework |
| Thursday | **Specialized Cloud Architecture Deep Dive Case Studies**<ul><li>Evaluated pure serverless backends (API Gateway + AWS Lambda + DynamoDB), contrasting cold-start latency characteristics and operational trade-offs against containerized ECS Fargate services.</li><li>Modeled hybrid asynchronous processing workflows pairing static S3 web hosting with SQS background queues for resilient, decoupled enterprise scaling.</li></ul> | Dec 10, 2026 | Dec 10, 2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Specialized Use Cases |
| Friday | **End-to-End System Verification & Demo Video Validation**<ul><li>Executed end-to-end operational verification across Tindy's deployed CloudFront distribution: user onboarding, project publishing, applicant review, live SignalR chat, and Bedrock AI CV extraction.</li><li>Validated the official 7m 22s application demonstration recording, cross-referencing UI frame captures and verifying production readiness across all modules.</li></ul> | Dec 11, 2026 | Dec 11, 2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Well-Architected Solutions<br>03 — AWS Well-Architected Framework<br>04 — Specialized Use Cases |
| Monday (Dec 14) | **Internship Wrap-Up & Final Bilingual Documentation**<ul><li>Completed personal internship documentation: finalized 13-week worklogs, self-evaluations, and program feedback reflecting Cao Thành Nhân's unique engineering growth.</li><li>Audited bilingual navigation consistency (English and Vietnamese), ensuring project summary Markdown and draw.io XML architectural assets met all FCAJ guidelines.</li></ul> | Dec 14, 2026 | Dec 14, 2026 | Internship report |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

Week 13 marks the culmination of an enriching internship journey in the AWS Workforce Bootcamp - First Cloud AI Journey. Reflecting on this path—from initial explorations of IAM, VPCs, and EC2 to co-architecting and deploying a resilient, modern cloud application like Tindy—has been truly transformative.

Evaluating our application against the six Well-Architected pillars cemented a comprehensive engineering mindset: great software craftsmanship extends beyond functional code into operational reliability, security boundaries, cost discipline, and scalability. Hands-on experience with React, TypeScript, CORS hardening, message rate limiting, and AWS cloud infrastructure represents the ultimate foundation for my software engineering career.

### Week 13 Learning Outcomes

- The six pillars of the AWS Well-Architected Framework serve as the definitive standard for architecting and assessing enterprise-grade cloud systems.
- This internship solidified modern full-stack web engineering disciplines while developing practical, real-world cloud architectural thinking.
- Application in Tindy: Assessed Tindy against the 6 Well-Architected pillars; finalized end-to-end UI verification and Workshop Section 5.6 demo scenarios.
