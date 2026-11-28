---
title: "Week 6 Worklog"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

**Module 6** — Cloud Storage Services (Amazon S3, EBS, EFS) and Asset Management

### Week 6 Objectives

- Differentiate the three core storage archetypes: Object Storage (Amazon S3), Block Storage (Amazon EBS), and File Storage (Amazon EFS).
- Evaluate Amazon S3 Storage Classes and configure automated S3 Lifecycle Rules to achieve long-term storage cost optimization.
- Master static website hosting on S3, secure bucket policies with Origin Access Control (OAC), and implement direct client uploads using S3 Presigned URLs.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Object Storage Architecture with Amazon S3**<ul><li>Explored Amazon S3 fundamentals: virtually unlimited object storage engineered for 99.999999999% (11 9s) of data durability across multiple facilities.</li><li>Analyzed S3 Bucket structures: globally unique naming, virtual directory key hierarchies, object metadata headers, and S3 Versioning preventing accidental deletions.</li></ul> | Oct 19, 2026 | Oct 19, 2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Storage |
| Tuesday | **S3 Storage Classes & Automated Lifecycle Transitions**<ul><li>Contrasted S3 tiers: S3 Standard (frequent access), S3 Standard-IA (infrequent access), and S3 Glacier tiers (low-cost archival with varying retrieval windows).</li><li>Investigated S3 Intelligent-Tiering: automatically shifting objects across access tiers without retrieval fees; configured S3 Lifecycle Rules to archive dormant resume PDFs after 90 days.</li></ul> | Oct 20, 2026 | Oct 20, 2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — EC2 Instance Store and Amazon Elastic Block Store (Amazon EBS) |
| Wednesday | **Block Storage (EBS) vs Shared Network File Systems (EFS)**<ul><li>Investigated Amazon Elastic Block Store (EBS): dedicated block volumes attached to virtual instances, supporting point-in-time EBS Snapshots and hardware encryption.</li><li>Compared EBS with Amazon Elastic File System (EFS): managed NFS storage enabling concurrent multi-attach read/write operations across distributed containers.</li></ul> | Oct 21, 2026 | Oct 21, 2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Amazon Elastic Block Store (Amazon EBS) Data Lifecycle |
| Thursday | **Static Web Hosting & Direct S3 Presigned URL Uploads**<ul><li>Evaluated S3 static website hosting workflows: configuring `index.html` entry points and custom routing error documents for Single Page Applications (SPAs).</li><li>Analyzed direct client-to-storage patterns: frontend React clients request short-lived cryptographic Presigned URLs from the backend, uploading heavy PDF files directly to S3 without choking API server bandwidth.</li></ul> | Oct 22, 2026 | Oct 22, 2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Amazon Simple Storage Service (Amazon S3) |
| Friday | **S3 Security Hardening: Block Public Access & OAC**<ul><li>Examined Amazon S3 Block Public Access settings, preventing unauthorized public data leaks at both account and bucket levels.</li><li>Configured fine-grained S3 Bucket Policies paired with CloudFront Origin Access Control (OAC): restricting S3 object read access exclusively to the designated CloudFront CDN distribution.</li></ul> | Oct 23, 2026 | Oct 23, 2026 | [AWS Skill Builder — Module 6](https://skillbuilder.aws/renderer/?module_id=18SQAPSR8X%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Amazon S3 Storage Classes and S3 Lifecycle<br>06 — Amazon S3 Demonstration |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

Week 6 unlocked a crucial architectural breakthrough for Tindy: direct uploads via S3 Presigned URLs. In traditional web development, I often dispatched file binaries to backend endpoints via `multipart/form-data`, which readily consumed server memory and throttled network I/O during concurrent uploads.

Leveraging S3 Presigned URLs completely transformed this workflow. My React frontend fetches an ephemeral cryptographically signed URL from our backend, then streams the PDF directly into S3 using a standard HTTP PUT request. This eliminates backend bottlenecks and provides an instant, responsive upload experience for students submitting resumes.

### Week 6 Learning Outcomes

- Amazon S3 provides virtually unbreakable durability with versatile storage tiers that automatically optimize cost lifecycles.
- Presigned URLs provide an industry-standard pattern for secure, high-throughput client-to-storage direct ingestion.
- Application in Tindy: Deployed the production React bundle to S3; evaluated Presigned URL workflows for direct student CV PDF uploads.
