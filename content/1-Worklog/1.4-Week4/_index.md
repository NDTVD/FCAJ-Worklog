---
title: "Week 4 Worklog"
date: 2024-01-01
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

**Module 4** — AWS Regions, Edge Locations, and Infrastructure as Code (CloudFormation)

### Week 4 Objectives

- Evaluate multi-factor criteria for selecting optimal AWS Regions (geographic latency, compliance requirements, service availability, and cost models).
- Understand the critical role of Edge Locations and Amazon CloudFront Content Delivery Networks (CDN) in frontend delivery acceleration.
- Master Infrastructure as Code (IaC) fundamentals via AWS CloudFormation: templates, stacks, change sets, and automated rollback triggers.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Global Infrastructure Distribution & Region Selection**<ul><li>Evaluated four foundational criteria for AWS Region selection: 1) Data governance and compliance mandates; 2) Proximity and round-trip network latency to end users; 3) Regional service availability (e.g., Amazon Bedrock regional availability); 4) Pricing variations across geographical locations.</li><li>Analyzed why US East (N. Virginia, us-east-1) serves as an optimal baseline for student demos and technology prototypes due to comprehensive feature sets and competitive costs.</li></ul> | Oct 05, 2026 | Oct 05, 2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Going Global |
| Tuesday | **Edge Presence & Amazon CloudFront Acceleration**<ul><li>Investigated AWS's global network of over 600 Points of Presence (Edge Locations). Analyzed CDN caching mechanics: serving static assets from edge caches nearest to client request origins.</li><li>Evaluated origin offloading techniques and automated SSL/TLS termination utilizing integrated AWS Certificate Manager (ACM) certificates.</li></ul> | Oct 06, 2026 | Oct 06, 2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — Choosing AWS Regions |
| Wednesday | **Infrastructure as Code (IaC) Paradigms**<ul><li>Studied core advantages of codified infrastructure: declarative repeatability, auditability through Git versioning, elimination of manual configuration drift, and rapid environment cloning across stages.</li><li>Contrasted imperative Console provisioning against declarative JSON/YAML infrastructure modeling.</li></ul> | Oct 07, 2026 | Oct 07, 2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Diving Deeper into AWS Global Infrastructure |
| Thursday | **CloudFormation Syntax, Stacks & Change Sets**<ul><li>Analyzed structural CloudFormation sections: AWSTemplateFormatVersion, input Parameters, mandatory Resources block, and exported Outputs for cross-stack references.</li><li>Examined Change Sets for pre-execution impact assessment, Drift Detection for identifying out-of-band modifications, and automated rollback workflows on provisioning failure.</li></ul> | Oct 08, 2026 | Oct 08, 2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Infrastructure and Automation |
| Friday | **Multi-Stack Infrastructure Architecture Design**<ul><li>Explored decoupling monolithic templates into modular layers: Foundation, Network, Database, Integrations, Runtime, and Edge.</li><li>Evaluated cross-stack parameter injection: passing Network Outputs (VpcId, SubnetIds) into Database and Runtime input parameters to preserve modular boundaries.</li></ul> | Oct 09, 2026 | Oct 09, 2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — Choosing AWS Regions<br>04 — Infrastructure and Automation |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

Module 4 demystified Infrastructure as Code (IaC) through AWS CloudFormation. Seeing dozens of cloud resources defined declaratively within YAML templates highlighted the value of repeatable deployments over manual AWS Console clicks.

For web development, the lessons on Edge Locations and CloudFront were especially relevant. I learned that rather than forcing clients to fetch JavaScript bundles and CSS assets directly from Virginia servers, CloudFront caches them at edge locations worldwide, drastically reducing initial page load times for Vietnamese users.

### Week 4 Learning Outcomes

- Infrastructure as Code represents a non-negotiable software engineering discipline for repeatable provisioning and teardown automation.
- Amazon CloudFront paired with Edge Locations maximizes origin offload while optimizing client delivery latency worldwide.
- Application in Tindy: Selected us-east-1 for unified deployment; studied how CloudFront distributes static React bundles with minimal latency.
