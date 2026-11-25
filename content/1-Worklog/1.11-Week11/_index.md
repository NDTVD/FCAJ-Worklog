---
title: "Week 11 Worklog"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

**Module 11** — AWS pricing, support, and cost optimization

### Week 11 Objectives

- Identify application cost drivers and explain when usage commitments may be worth considering.
- Read cost data, allocate costs with tags, and design budget alerts.
- Compare technical support needs and evaluate optimization options using usage data.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Pricing models and cost drivers**<ul><li>Distinguish pay-as-you-go, savings through commitments, and tiered rates. List the three basic cost categories: compute, storage, and outbound data transfer.</li><li>Compare a Tindy demo run with always-on operation. Record Fargate and RDS hours, ALB lifetime, S3 storage, logs, and snapshots to see which items continue accruing charges between demos.</li></ul> | Nov 23, 2026 | Nov 23, 2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Pricing and Support<br>02 — AWS Pricing Concepts |
| Tuesday | **Billing Dashboard, AWS Budgets, and Cost Explorer**<ul><li>Distinguish where to view current charges, analyze trends, and configure alerts. Review actual and forecast cost examples in AWS Budgets.</li><li>Sketch cost groupings by service, account, and project tag. Identify which tags must be activated for cost allocation, then relate consolidated billing to reviewing charges across accounts.</li></ul> | Nov 24, 2026 | Nov 24, 2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — AWS Pricing and Billing Services |
| Wednesday | **Assessing AWS Support needs**<ul><li>Compare account and billing support with technical support for a running workload. Use the lesson scenarios to identify impact and response needs.</li><li>Draft a support case with symptoms, timing, Region, impact, and checks already performed. Distinguish initial response time from time to resolution.</li></ul> | Nov 25, 2026 | Nov 25, 2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — AWS Support Plans |
| Thursday | **AWS Marketplace and AWS Partner Network**<ul><li>Distinguish sourcing products or services through AWS Marketplace from finding implementation, integration, or migration expertise through the AWS Partner Network.</li><li>Evaluate a third-party tool by its pricing model, terms, permissions, and operational work. Separate vendor charges from AWS infrastructure charges incurred while running it.</li></ul> | Nov 26, 2026 | Nov 26, 2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — AWS Marketplace and AWS Partners |
| Friday | **Optimizing costs using usage data**<ul><li>Review examples of compute rightsizing, RDS utilization checks, and S3 lifecycle selection. Examine transfer paths and when an S3 gateway endpoint can replace a NAT path in a suitable architecture.</li><li>Outline a cycle for measuring current cost, selecting one change, tracking its effect, and checking performance afterward. Prioritize demo resources that do not require continuous operation and list the data needed for recovery.</li></ul> | Nov 27, 2026 | Nov 27, 2026 | [AWS Skill Builder — Module 11](https://skillbuilder.aws/renderer/?module_id=UGUXWW6BEZ%3A002.001.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Cost Optimization |

### Week 11 Learning Outcomes

- Application cost depends on runtime and resources retained between runs.
- Billing Dashboard, Budgets, and Cost Explorer support reviewing charges, receiving alerts, and analyzing trends.
- An optimization proposal needs before-and-after measurements, operating expectations, and a data preservation plan.
- **Application in Tindy:** Practiced cost modeling with AWS Pricing Calculator (~.32/mo) and adopted scheduled demo teardowns to keep actual costs under .

