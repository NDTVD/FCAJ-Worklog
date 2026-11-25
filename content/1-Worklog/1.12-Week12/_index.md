---
title: "Week 12 Worklog"
date: 2024-01-01
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

**Module 12** — AWS migration strategies and data transfer

### Week 12 Objectives

- Describe the migration phases and how AWS CAF helps prepare an organization.
- Choose a strategy from the 7 Rs and identify suitable application or database migration tools.
- Compare online and offline data transfer based on volume, timing, and bandwidth.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Migration phases and AWS CAF**<ul><li>List the work in Assess, Mobilize, and Migrate and Modernize. Use a .NET backend to identify dependencies such as PostgreSQL, file storage, and authentication before moving.</li><li>Map preparation tasks to the six AWS CAF perspectives: Business, People, Governance, Platform, Security, and Operations. Identify who owns assessment, preparation, and ongoing operations.</li></ul> | Nov 30, 2026 | Nov 30, 2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Migration<br>02 — AWS Cloud Adoption Framework |
| Tuesday | **The seven migration strategies and tools**<ul><li>Compare rehost, relocate, replatform, refactor, repurchase, retain, and retire. Use a move from self-managed PostgreSQL to RDS to explain replatforming.</li><li>Review the roles of dependency discovery, cost modeling, server migration, and progress tracking. Compare AWS Application Migration Service with planning tools and place the services covered in the transcript in their lesson context.</li></ul> | Dec 1, 2026 | Dec 1, 2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Seven Migration Strategies<br>04 — Migration Services and Tools |
| Wednesday | **Database migration with AWS DMS**<ul><li>Distinguish homogeneous from heterogeneous migrations. Identify when schema conversion is required and the roles of AWS DMS and schema conversion tooling.</li><li>Outline a PostgreSQL migration with an initial full load, change data capture where appropriate, record counts, and transaction checks before cutover. Define when to stop or return to the source if verification fails.</li></ul> | Dec 2, 2026 | Dec 2, 2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Database Migrations |
| Thursday | **Online data transfer**<ul><li>Compare DataSync for moving datasets between storage systems, Transfer Family for receiving files over supported protocols, and Direct Connect for dedicated connectivity.</li><li>Estimate copy time for a media directory from volume and effective throughput. Distinguish a one-time file transfer from long-term connectivity and define checks for the files at the destination.</li></ul> | Dec 3, 2026 | Dec 3, 2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Transferring Data Online |
| Friday | **Offline data transfer and trade-offs**<ul><li>Review the Snowball Edge example in the notes to understand copying data to a device, shipping it, and importing it into AWS. Relate edge processing to environments with unreliable connectivity.</li><li>Compare copying, shipping, and import time with an online transfer. In the sample plan, note the need to verify service availability and choose how to validate data integrity after the move.</li></ul> | Dec 4, 2026 | Dec 4, 2026 | [AWS Skill Builder — Module 12](https://skillbuilder.aws/renderer/?module_id=P6BSGWZVFE%3A001.000.003&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>07 — Transferring Data Offline |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

Module 12's exploration of cloud migration frameworks (7Rs) and application modernization highlighted the necessity of release automation.

In Tindy, I contributed to configuring GitHub Actions CI/CD workflows using passwordless AWS OIDC authentication. Whenever frontend changes are committed to main, the workflow executes npm run build, synchronizes the dist/ directory to S3, and issues a CloudFront cache invalidation, delivering UI updates globally in under two minutes.

### Week 12 Learning Outcomes

- Dependency inventory and the AWS CAF perspectives help define what needs to be ready before cutover.
- The 7 Rs distinguish how much an application changes. Schema conversion, initial load, and change replication need separate planning.
- Transfer estimates need to account for effective throughput, downtime, and post-migration reconciliation.
- **Application in Tindy:** Established GitHub Actions OIDC CI/CD to automate React static bundling (npm run build), S3 upload, and CloudFront cache invalidation.


