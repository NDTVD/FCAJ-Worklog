---
title: "Week 12 Worklog"
date: 2024-01-01
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

**Module 12** — Cloud Migration Strategies (7 Rs), Application Modernization, and CI/CD Automation

### Week 12 Objectives

- Master cloud migration phases through the AWS Cloud Adoption Framework (CAF) and the 7 Rs migration decision tree.
- Evaluate online (AWS DataSync, Transfer Family) and offline (AWS Snow Family) data transfer mechanisms based on bandwidth and volume.
- Establish continuous integration and continuous deployment (CI/CD) pipelines using GitHub Actions and AWS OIDC for automated web delivery.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **AWS Cloud Adoption Framework (CAF) & Migration Phases**<ul><li>Explored the three cloud transformation phases: Assess, Mobilize, and Migrate and Modernize.</li><li>Mapped migration planning against the six AWS CAF perspectives: Business, People, Governance, Platform, Security, and Operations to ensure organizational alignment.</li></ul> | Nov 30, 2026 | Nov 30, 2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Migration<br>02 — AWS Cloud Adoption Framework |
| Tuesday | **The 7 Rs Migration Decision Matrix & Modernization**<ul><li>Evaluated the 7 Rs strategies: Rehost, Relocate, Replatform, Refactor, Repurchase, Retain, and Retire.</li><li>Analyzed application modernization journeys: transitioning legacy monolithic codebases into containerized microservices (Replatform/Refactor) hosted on AWS Fargate paired with decoupled static S3 clients.</li></ul> | Dec 01, 2026 | Dec 01, 2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Seven Migration Strategies<br>04 — Migration Services and Tools |
| Wednesday | **Database Migration Mechanics with AWS DMS**<ul><li>Investigated AWS Database Migration Service (DMS): enabling seamless database migrations with near-zero application downtime.</li><li>Contrasted homogeneous database migrations (PostgreSQL to Amazon RDS PostgreSQL) with heterogeneous migrations using AWS Schema Conversion Tool (SCT); studied ongoing replication via Change Data Capture (CDC).</li></ul> | Dec 02, 2026 | Dec 02, 2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Database Migrations |
| Thursday | **Online vs Offline Data Transfer Strategies**<ul><li>Contrasted online network transfer solutions: AWS DataSync (accelerated file synchronization to S3/EFS), AWS Transfer Family (managed SFTP), and dedicated AWS Direct Connect circuits.</li><li>Examined offline edge appliances: AWS Snowcone, Snowball Edge, and Snowmobile for multi-terabyte to petabyte data transport where network bandwidth constraints prevail.</li></ul> | Dec 03, 2026 | Dec 03, 2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Transferring Data Online |
| Friday | **Automated Deployment via GitHub Actions CI/CD & AWS OIDC**<ul><li>Engineered automated release pipelines: triggering automated testing, bundling, and deployment workflows upon git pushes to the `main` branch.</li><li>Configured GitHub Actions workflows: executing `npm run build`, authenticating to AWS via temporary OIDC identity federation, syncing build artifacts to S3, and issuing CloudFront cache invalidations.</li></ul> | Dec 04, 2026 | Dec 04, 2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>07 — Transferring Data Offline |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

Module 12 on cloud migration strategies (7 Rs) and application modernization fundamentally reshaped my engineering workflow regarding software release automation. Previously, deploying frontend updates involved running local builds and manually uploading files via FTP or management consoles—a brittle, error-prone routine.

For Tindy, I helped establish an automated CI/CD deployment pipeline utilizing GitHub Actions paired with passwordless AWS OIDC authentication. Whenever frontend changes are merged into the main branch, our workflow automatically builds the React distribution, synchronizes static bundles to our S3 bucket, and triggers CloudFront cache invalidations—delivering global UI updates in under 90 seconds.

### Week 12 Learning Outcomes

- The AWS Cloud Adoption Framework and the 7 Rs provide a disciplined roadmap for modernizing legacy systems into agile cloud architectures.
- Automated CI/CD pipelines backed by passwordless AWS OIDC authentication eliminate credential risks while maximizing deployment velocity.
- Application in Tindy: Established GitHub Actions OIDC CI/CD to automate React static bundling (npm run build), S3 upload, and CloudFront cache invalidation.
