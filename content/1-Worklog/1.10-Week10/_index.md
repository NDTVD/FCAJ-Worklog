---
title: "Week 10 Worklog"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

**Module 10** — Monitoring (CloudWatch), Audit Logging (CloudTrail), and Frontend Observability

### Week 10 Objectives

- Master telemetry with Amazon CloudWatch: metrics aggregation, centralized container logging, and visual infrastructure dashboards.
- Configure automated threshold alarms (CloudWatch Alarms) dispatching operational notifications via Amazon SNS.
- Combine AWS CloudTrail audit histories with client-side browser performance profiling to rapidly diagnose cross-stack issues.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Telemetry Collection with Amazon CloudWatch Metrics**<ul><li>Surveyed standard system metrics: ECS CPUUtilization and MemoryUtilization, ALB target response latency, HTTP 5XX rates, and RDS database connections.</li><li>Constructed centralized CloudWatch Dashboards: graphing real-time operational telemetry to provide unified health visibility across our application stack.</li></ul> | Nov 16, 2026 | Nov 16, 2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Monitoring, Compliance, and Governance in the AWS Cloud<br>02 — Introduction to Monitoring<br>03 — Amazon CloudWatch |
| Tuesday | **Centralized Container Logging via CloudWatch Logs**<ul><li>Analyzed ECS container log routing using the native `awslogs` driver: aggregating stdout/stderr streams into dedicated CloudWatch Log Groups.</li><li>Executed CloudWatch Logs Insights queries: filtering stack traces and unhandled ASP.NET Core exceptions to pinpoint root causes behind intermittent API failures.</li></ul> | Nov 17, 2026 | Nov 17, 2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — AWS CloudTrail |
| Wednesday | **Automated Incident Alarms & SNS Alert Dispatch**<ul><li>Configured metric alarm thresholds: triggering alerts when HTTP 5XX error rates breach 5% over consecutive evaluation periods or container memory exceeds 85%.</li><li>Tied alarm states directly to Amazon SNS topics: dispatching automated incident email alerts to developers and signaling auto-scaling policies.</li></ul> | Nov 18, 2026 | Nov 18, 2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Compliance<br>06 — Auditing AWS Resources for Compliance |
| Thursday | **Governance & Security Auditing with AWS CloudTrail**<ul><li>Investigated AWS CloudTrail: continuously logging API actions and resource state mutations across AWS management consoles and programmatic SDK calls.</li><li>Analyzed CloudTrail event payloads: inspecting identity callers, origin IP addresses, request parameters, and response elements for compliance auditing.</li></ul> | Nov 19, 2026 | Nov 19, 2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>07 — AWS Organizations<br>08 — Governance |
| Friday | **Frontend Observability & Client-Side Resiliency**<ul><li>Profiled browser network flows via Chrome DevTools: tracking Time to First Byte (TTFB), static bundle parsing durations, and WebSocket handshake latencies.</li><li>Engineered robust React Error Boundaries: isolating component runtime crashes to prevent application-wide white screens while displaying informative recovery prompts.</li></ul> | Nov 20, 2026 | Nov 20, 2026 | [AWS Skill Builder — Module 10](https://skillbuilder.aws/renderer/?module_id=HU3PMBK47Y%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>09 — AWS Health<br>10 — AWS Trusted Advisor |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

Module 10 broadened my understanding of end-to-end full-stack observability. Reliable software engineering requires continuous telemetry and automated alerting in production environments rather than relying on local assumptions.

On the frontend, this highlighted the importance of graceful degradation. When backend services experience temporary faults or return 500 errors, unhandled exceptions must not crash the entire React application into a blank white viewport. Implementing robust Error Boundaries with contextual retry buttons preserved an exceptional user experience even during underlying service recovery.

### Week 10 Learning Outcomes

- Amazon CloudWatch acts as the core observability nerve center, aggregating telemetry, logs, and automated incident alarms.
- AWS CloudTrail guarantees immutable governance audit trails for all programmatic and console infrastructure modifications.
- Application in Tindy: Utilized browser DevTools to analyze API latency; implemented React Error Boundaries to preserve UI resilience during runtime anomalies.
