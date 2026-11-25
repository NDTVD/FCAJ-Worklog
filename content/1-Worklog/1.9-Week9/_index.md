---
title: "Week 9 Worklog"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

**Module 9** — Security, data protection, and incident response

### Week 9 Objectives

- Distinguish authentication, authorization, and AWS and customer responsibilities.
- Choose safeguards at the network, application, and data layers.
- Identify the role of each service in detection and investigation.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Identity and access control**<ul><li>Distinguish authentication from authorization using a Tindy user signing in and then requesting a resource. Review root account protection with MFA and appropriate identities for regular tasks.</li><li>Read IAM policies in terms of principals, actions, and resources. Use an ECS task role accessing S3 as a least-privilege scenario, then compare it with human access through IAM Identity Center.</li></ul> | Nov 9, 2026 | Nov 9, 2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Security on AWS<br>02 — Preventing Unauthorized Access |
| Tuesday | **Network and application protection**<ul><li>Trace CloudFront, the ALB, and ECS to identify the traffic each security group needs to allow.</li><li>Compare AWS WAF filtering at the application layer with AWS Shield protection against DDoS. Identify which components belong to the course's defense-in-depth example when relating it to Tindy's architecture.</li></ul> | Nov 10, 2026 | Nov 10, 2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Protecting Networks and Applications |
| Wednesday | **Encryption and data protection**<ul><li>Distinguish encryption at rest in S3 or EBS from encryption in transit through TLS. Use a document upload to identify the points the data passes through.</li><li>Compare AWS KMS key management with ACM certificate management. Identify the permissions to check for encrypted data access, including resource access and permission to use the key where applicable.</li></ul> | Nov 11, 2026 | Nov 11, 2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Protecting Data |
| Thursday | **Detection and incident investigation**<ul><li>Map the roles of Inspector for vulnerability findings, GuardDuty for threat findings, Detective for investigation, and Security Hub for consolidated security visibility.</li><li>Use a sample finding to identify the resource, time, and evidence to check. Link finding triage to impact verification before choosing a response.</li></ul> | Nov 12, 2026 | Nov 12, 2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Detecting and Responding to Security Incidents |
| Friday | **Reviewing security resources**<ul><li>Identify when to use AWS documentation for configuration, Knowledge Center for troubleshooting, and the AWS Security Blog for implementation context.</li><li>Review a scenario for adopting a security solution from AWS Marketplace. Evaluate permissions, cost, operating responsibilities, and infrastructure fit before selecting it.</li></ul> | Nov 13, 2026 | Nov 13, 2026 | [AWS Skill Builder — Module 9](https://skillbuilder.aws/renderer/?module_id=TNAPD78T9R%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Additional Security Resources |

### Week 9 Learning Outcomes

- IAM and least privilege limit what each identity or workload can do.
- Security groups, WAF, Shield, TLS, and encryption at rest serve different protection layers.
- A security finding is an input to verifying the affected resource, timeline, and impact.
- **Application in Tindy:** Personally configured CORS in ASP.NET Core for secure CloudFront API access and implemented backend Message Rate Limiting against chat spam.

