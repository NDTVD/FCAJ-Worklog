---
title: "Week 6 Worklog"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

**Module 6** — AWS storage, EBS, and S3

### Week 6 Objectives

- Choose block, object, or file storage based on how an application accesses data.
- Distinguish EC2 instance store from Amazon EBS and explain snapshot and retention policies.
- Explain Amazon S3 structure and choose suitable storage classes and transition or expiration rules.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Block, object, and file storage**<ul><li>Compare block, object, and file storage through examples with Amazon EBS, Amazon S3, and Amazon EFS.</li><li>Compare three access models: block devices, objects by key, and shared filesystem files. Use a database on EC2, user uploads, and a shared directory to choose among EBS, S3, and EFS.</li></ul> | Oct 19, 2026 | Oct 19, 2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Storage |
| Tuesday | **EC2 instance store and Amazon EBS**<ul><li>Compare EC2 instance store and Amazon EBS by data persistence across instance state changes.</li><li>Build a reboot, stop, and terminate comparison for instance store and EBS. Identify when temporary files fit instance store, when a persistent volume is needed, and which setting affects EBS retention on termination.</li></ul> | Oct 20, 2026 | Oct 20, 2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — EC2 Instance Store and Amazon Elastic Block Store (Amazon EBS) |
| Wednesday | **Snapshots and the EBS lifecycle**<ul><li>Review incremental snapshots, restoring volumes from snapshots, and backup automation with Amazon Data Lifecycle Manager.</li><li>Draw a snapshot timeline showing changed blocks across backups. Explain how to create a new volume from a recovery point and outline a DLM policy with snapshot timing and retention.</li></ul> | Oct 21, 2026 | Oct 21, 2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Amazon Elastic Block Store (Amazon EBS) Data Lifecycle |
| Thursday | **Amazon S3 buckets, objects, and metadata**<ul><li>Review buckets, objects, keys, and metadata. Distinguish durability from availability.</li><li>Describe how a bucket contains objects, a key identifies an object, and metadata describes it. Use a profile file to distinguish permission to read it, availability at a given time, and long-term durability.</li></ul> | Oct 22, 2026 | Oct 22, 2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Amazon Simple Storage Service (Amazon S3) |
| Friday | **Storage classes, S3 Lifecycle, and the S3 demo**<ul><li>Compare storage classes by access frequency, retrieval time, and cost. Review S3 Lifecycle transitions and object expiration. Review the demo for creating a bucket, uploading an object, inspecting metadata, and examining bucket policy and S3 Versioning.</li><li>Choose storage classes for frequently viewed images, infrequently accessed data, and long-term archives. Draft a Lifecycle example with transition and expiration dates. Cross-check the console demo for the bucket, object, and version information to inspect.</li></ul> | Oct 23, 2026 | Oct 23, 2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Amazon S3 Storage Classes and S3 Lifecycle<br>06 — Amazon S3 Demonstration |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

As a frontend developer, Amazon S3 is the AWS service I engage with most frequently. This week clarified the distinctions between block storage (EBS) and object storage (S3).

I applied this directly to project Tindy by defining two separate S3 storage roles: one private bucket for static React bundles governed by Origin Access Control (OAC), and a dedicated S3 Media bucket for avatars and candidate resumes. Learning about S3 Lifecycle policies also gave me practical ideas for automated temporary file cleanup to optimize storage costs.

### Week 6 Learning Outcomes

- Instance store suits temporary data, EBS persists data according to the volume lifecycle, and snapshots provide recovery points.
- Choose storage classes based on data access requirements. S3 Lifecycle automates object transitions and expiration.
- **Application in Tindy:** Configured Amazon S3 for static frontend hosting (via OAC) and private S3 Media storage for uploaded candidate resumes.


