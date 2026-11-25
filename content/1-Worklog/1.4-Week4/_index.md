---
title: "Week 4 Worklog"
date: 2024-01-01
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

**Module 4** — AWS Regions and infrastructure automation

### Week 4 Objectives

- Distinguish the roles of Regions, Availability Zones, and edge locations in serving global users.
- Evaluate Regions against user location, compliance, service availability, and cost.
- Explain how AWS CloudFormation describes infrastructure, deploys it, and tracks changes.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Deploying for global users**<ul><li>Review the roles of Regions and edge locations in serving global users.</li><li>Distinguish where a backend runs from where content is delivered near users. Draw a request from the browser to edge content and then to the application in a Region, noting how each location affects latency.</li></ul> | Oct 5, 2026 | Oct 5, 2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Going Global |
| Tuesday | **AWS Region selection criteria**<ul><li>Evaluate Region choices based on compliance, proximity to users, service availability, and cost.</li><li>Build a Region selection matrix for an application serving two user groups. Mark mandatory data residency and service availability requirements before comparing latency and cost among the remaining options.</li></ul> | Oct 6, 2026 | Oct 6, 2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — Choosing AWS Regions |
| Wednesday | **Resource placement in AWS infrastructure**<ul><li>Review Regions, Availability Zones, and edge locations from an application deployment perspective.</li><li>Use an application spanning two AZs to distinguish choosing a Region from placing resources inside it. Explain when AZ redundancy is needed and when an application might need to serve users from multiple Regions.</li></ul> | Oct 7, 2026 | Oct 7, 2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Diving Deeper into AWS Global Infrastructure |
| Thursday | **Templates, stacks, and change management**<ul><li>Review CloudFormation templates and stacks and the roles of change sets, drift detection, and StackSets.</li><li>Annotate a template's parameters, resources, and outputs. Map each task to the relevant feature: preview changes with a change set, identify differences with drift detection, and use StackSets to manage deployments across accounts or Regions.</li></ul> | Oct 8, 2026 | Oct 8, 2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Infrastructure and Automation |
| Friday | **Region selection scenario and deployment settings**<ul><li>Choose a Region for a sample application, justify it using the selection criteria, and outline the parameters needed in a CloudFormation template.</li><li>Turn the Region decision into repeatable deployment settings. Distinguish fixed template values from parameters supplied at stack creation. Use the proposed parameters and outputs to prepare for the following week's lab.</li></ul> | Oct 9, 2026 | Oct 9, 2026 | [AWS Skill Builder — Module 4](https://skillbuilder.aws/renderer/?module_id=VEE8JSBK3Z%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — Choosing AWS Regions<br>04 — Infrastructure and Automation |

### Week 4 Learning Outcomes

- Region selection balances latency with data residency requirements, service features, and cost.
- CloudFormation templates describe infrastructure, and stacks manage the resources deployed from those templates.
- **Application in Tindy:** Selected us-east-1 for unified deployment; studied how CloudFront distributes static React bundles with minimal latency.

