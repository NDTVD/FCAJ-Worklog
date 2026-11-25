---
title: "Week 3 Worklog"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

**Module 3** — Serverless, containers, and compute services

### Week 3 Objectives

- Compare operational responsibilities across EC2, managed services, and serverless.
- Explain AWS Lambda event processing, including the trigger, handler, and execution permissions.
- Choose container or specialized compute services based on deployment and workload needs.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Serverless and operational responsibilities**<ul><li>Compare EC2, managed services, and serverless by infrastructure control and operational effort.</li><li>Compare the operational work that remains when running an application on EC2, using a managed service, or adopting serverless. Build a short matrix for server management, capacity scaling, code deployment, and application permissions.</li></ul> | Sep 28, 2026 | Sep 28, 2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Serverless Computing |
| Tuesday | **Event processing with AWS Lambda**<ul><li>Review Lambda triggers, events, handlers, and execution permissions through an S3 upload example.</li><li>Trace an S3 upload. Identify the event source, the information passed to the function, the handler, and the permissions needed to read or write data. Note how execution duration affects the decision to use Lambda.</li></ul> | Sep 29, 2026 | Sep 29, 2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — AWS Lambda |
| Wednesday | **Containers and orchestration**<ul><li>Distinguish containers from virtual machines and review the roles of Amazon ECS, Amazon EKS, Amazon ECR, and AWS Fargate.</li><li>Compare packaging and environment consistency for the same application deployed as a VM and as a container. Diagram an image moving from ECR to an ECS or EKS workload, then annotate EC2 and Fargate as compute options.</li></ul> | Sep 30, 2026 | Sep 30, 2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Containers and Orchestration on AWS |
| Thursday | **Additional compute services**<ul><li>Compare AWS Elastic Beanstalk, AWS Batch, Amazon Lightsail, and AWS Outposts by use case.</li><li>List four needs: deploying a web app, running batch jobs, using a simple server, and operating AWS infrastructure on premises. Match each to a service from the lesson and identify what the application team still manages.</li></ul> | Oct 1, 2026 | Oct 1, 2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Additional Compute Services |
| Friday | **Scenario review for compute selection**<ul><li>Review Module 3 through three scenarios: processing file uploads, running a containerized app, and executing a batch job. Choose a service for each and explain why.</li><li>For each review scenario, record task duration, inputs, and required control over the environment. Choose a compute option, explain it, and name an assumption that could change the choice. Use the file-processing case to prepare for the Lambda lab.</li></ul> | Oct 2, 2026 | Oct 2, 2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — AWS Lambda<br>03 — Containers and Orchestration on AWS<br>04 — Additional Compute Services |

### Week 3 Learning Outcomes

- Lambda suits event-driven workloads. Task duration and execution permissions are two factors to check when choosing Lambda.
- ECR stores container images, ECS and EKS orchestrate containers, and Fargate provides compute capacity to run them.
- **Application in Tindy:** Grasped packaging the ASP.NET Core backend into ECR Docker images and running serverless containers via ECS Fargate.

