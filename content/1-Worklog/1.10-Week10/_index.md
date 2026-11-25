---
title: "Week 10 Worklog"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

**Module 10** — Monitoring, compliance, and governance on AWS

### Week 10 Objectives

- Distinguish operational metrics, application logs, and API activity history.
- Identify AWS compliance evidence and evidence to gather from customer resources.
- Explain multi-account governance and how to act on operational recommendations.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Monitoring applications with Amazon CloudWatch**<ul><li>Distinguish monitoring, auditing, compliance, and governance. Use a spike in Tindy API 5xx responses to choose metrics, a log group, and a time window.</li><li>Outline a dashboard for healthy targets, error rate, and ECS CPU usage. Explain how an alarm evaluates a threshold and sends an SNS notification when investigation is needed.</li></ul> | Nov 16, 2026 | Nov 16, 2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Monitoring, Compliance, and Governance in the AWS Cloud<br>02 — Introduction to Monitoring<br>03 — Amazon CloudWatch |
| Tuesday | **Auditing activity with AWS CloudTrail**<ul><li>Read a sample event to identify who acted, which API was called, when it occurred, and which resource was involved. Compare management and data events.</li><li>Use a security group change or an ECS update through CI/CD to distinguish Event history from a trail that retains audit records. Note how to compare the change timestamp with errors observed in CloudWatch.</li></ul> | Nov 17, 2026 | Nov 17, 2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — AWS CloudTrail |
| Wednesday | **Compliance evidence and resource configuration**<ul><li>Distinguish AWS reports and agreements in Artifact from the application's own checks for configuration, policy, and data location.</li><li>Explain how AWS Config records configuration and evaluates resources against rules. Review how the course uses Audit Manager frameworks, controls, assessments, and evidence to organize an audit.</li></ul> | Nov 18, 2026 | Nov 18, 2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Compliance<br>06 — Auditing AWS Resources for Compliance |
| Thursday | **Multi-account AWS governance**<ul><li>Diagram AWS Organizations with a management account, member accounts, and OUs. Distinguish consolidated billing from permission management.</li><li>Use a separation between dev and production to explain how SCPs limit which permissions can be granted. Relate AWS Control Tower to landing zones, Account Factory, and controls for multi-account governance.</li></ul> | Nov 19, 2026 | Nov 19, 2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>07 — AWS Organizations<br>08 — Governance |
| Friday | **AWS Health and AWS Trusted Advisor**<ul><li>Use a Fargate maintenance notification to identify affected resources, timing, and suggested actions in AWS Health.</li><li>Compare an AWS Health event with a Trusted Advisor recommendation. Choose a cost or service-limit check, verify the affected resource, and record who owns the follow-up.</li></ul> | Nov 20, 2026 | Nov 20, 2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>09 — AWS Health<br>10 — AWS Trusted Advisor |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

Week 10 emphasized system observability and governance using Amazon CloudWatch and AWS CloudTrail. A robust application requires continuous operational visibility to detect performance anomalies before users are impacted.

During UI testing, I paired Chrome DevTools Network inspections with live CloudWatch log streams. While testing our rate-limiting middleware, I validated that when the client received 429 Too Many Requests, corresponding warning logs were recorded cleanly in CloudWatch.

### Week 10 Learning Outcomes

- CloudWatch shows operational health, while CloudTrail traces API activity.
- AWS Artifact provides AWS compliance documentation. AWS Config records and evaluates resource configuration against selected rules.
- AWS Organizations and Control Tower support common controls across accounts. AWS Health and Trusted Advisor provide inputs for operational follow-up.
- **Application in Tindy:** Combined Chrome DevTools Network inspection with CloudWatch Logs to verify WebSocket 101 status codes and detect 429 throttled requests.


