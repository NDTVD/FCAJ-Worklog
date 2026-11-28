---
title: "Week 11 Worklog"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

**Module 11** — Cloud Economics, Cost Estimation (Pricing Calculator), and Budget Optimization

### Week 11 Objectives

- Utilize the AWS Pricing Calculator to formulate granular monthly cost estimations across web application infrastructure stacks.
- Master AWS cost governance tools: AWS Cost Explorer, AWS Budgets, and automated cost alert thresholds.
- Formulate resource optimization strategies for demo environments: scheduled compute hibernation to eliminate idle spending.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Architecture Cost Modeling via AWS Pricing Calculator**<ul><li>Explored the AWS Pricing Calculator: modeling architectural infrastructure to generate itemized monthly expenditure projections.</li><li>Constructed Tindy's cost estimate: modeling S3 static storage, CloudFront egress traffic, a single ECS Fargate task (0.25 vCPU, 0.5 GB RAM), a db.t4g.micro RDS instance, and Amazon Bedrock token usage.</li></ul> | Nov 23, 2026 | Nov 23, 2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Pricing and Support<br>02 — AWS Pricing Concepts |
| Tuesday | **Cost Attribution & Analysis with AWS Cost Explorer**<ul><li>Investigated AWS Cost Explorer: inspecting historical daily spending trends segmented by AWS service and geographic region.</li><li>Implemented Cost Allocation Tags: applying `Project: Tindy` and `Environment: Demo` tags to accurately isolate sprint verification expenses.</li></ul> | Nov 24, 2026 | Nov 24, 2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — AWS Pricing and Billing Services |
| Wednesday | **Budget Governance & Proactive Alerts with AWS Budgets**<ul><li>Configured AWS Budgets: defining strict monthly spend boundaries for our student demo environment (capped at $15.00/month).</li><li>Established multi-threshold notifications: triggering SNS alerts when actual spend crosses 80% or forecasted spend exceeds 100% of allocated limits.</li></ul> | Nov 25, 2026 | Nov 25, 2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — AWS Support Plans |
| Thursday | **AWS Free Tier Optimization & Compute Savings Options**<ul><li>Audited AWS Free Tier offerings: 12-month free tiers (RDS db.t3/t4g.micro), always-free services (1M Lambda requests, CloudWatch metrics), and trial credits.</li><li>Compared Fargate On-Demand versus Fargate Spot allocations, realizing up to 70% cost savings for fault-tolerant testing tasks.</li></ul> | Nov 26, 2026 | Nov 26, 2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — AWS Marketplace and AWS Partners |
| Friday | **Resource Scheduling & Dormant Compute Optimization**<ul><li>Analyzed idle infrastructure waste: student demo environments only require live uptime during testing and evaluation sessions, rendering 24/7 compute unnecessary.</li><li>Enacted resource scheduling discipline: scaling down ECS tasks and pausing database compute outside testing windows to eliminate idle cloud overhead.</li></ul> | Nov 27, 2026 | Nov 27, 2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Cost Optimization |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

Prior to this internship, I held common apprehensions that cloud infrastructure could incur unexpected runaway expenses. Week 11 completely dispelled this uncertainty by establishing disciplined financial governance practices.

Cloud expenditures are fully manageable when forecasted early using the AWS Pricing Calculator and ring-fenced with AWS Budgets alarms. In Tindy, isolating our static React client on S3 and CloudFront (incurring negligible pennies) while running our backend on a minimal ECS Fargate task achieved immense cost efficiency: our entire evaluation lifecycle cost only a few dollars.

### Week 11 Learning Outcomes

- The AWS Pricing Calculator and AWS Budgets are vital instruments for financial planning and avoiding budget overruns.
- Decoupling static frontend assets (S3/CloudFront) from server compute is the most economically efficient web architecture pattern.
- Application in Tindy: Calculated monthly infrastructure projections; configured AWS Budgets alerts to guarantee our project remained strictly within budget.
