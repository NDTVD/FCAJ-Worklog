---
title: "Week 3 Worklog"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

**Module 3** — Serverless Computing and Container Orchestration

### Week 3 Objectives

- Master serverless execution paradigms with AWS Lambda and event-driven computing triggers.
- Understand Docker containerization packaging and image registry hosting on Amazon Elastic Container Registry (ECR).
- Compare container orchestration platforms Amazon ECS and Amazon EKS; evaluate the serverless operational advantages of AWS Fargate.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Serverless Architecture & AWS Lambda Mechanics**<ul><li>Explored serverless fundamentals: zero server management, automatic request-driven scaling, and millisecond execution billing.</li><li>Analyzed event sources: API Gateway HTTP invocations, S3 object uploads, and SQS queue consumers. Examined execution runtime bounds (15-minute maximum timeout) and cold-start optimization strategies.</li></ul> | Sep 28, 2026 | Sep 28, 2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Serverless Computing |
| Tuesday | **Containerization Fundamentals & Amazon ECR**<ul><li>Contrasted Virtual Machines with Containerization: containers share the host OS kernel, yielding lightweight disk footprints and sub-second initialization times.</li><li>Investigated Amazon Elastic Container Registry (ECR): configuring private repositories, image digest tagging linked to git commits, and IAM push permissions for CI/CD runners.</li></ul> | Sep 29, 2026 | Sep 29, 2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — AWS Lambda |
| Wednesday | **Container Orchestration: Amazon ECS vs Amazon EKS**<ul><li>Evaluated Amazon Elastic Container Service (ECS) as AWS's native, lightweight container orchestrator.</li><li>Compared ECS with Amazon Elastic Kubernetes Service (EKS) for Kubernetes-native environments. Analyzed ECS Task Definitions (vCPU, memory, networking, environment parameters) and ECS Services (desired task count management).</li></ul> | Sep 30, 2026 | Sep 30, 2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Containers and Orchestration on AWS |
| Thursday | **Serverless Container Execution with AWS Fargate**<ul><li>Differentiated self-managed EC2 launch types from serverless AWS Fargate compute layers within Amazon ECS.</li><li>Analyzed Fargate operational automation: developers allocate discrete vCPU and memory slices per task, while AWS autonomously manages underlying infrastructure patching and hypervisor isolation.</li></ul> | Oct 01, 2026 | Oct 01, 2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Additional Compute Services |
| Friday | **Multi-Tier Containerized Web Application Modeling**<ul><li>Drafted an end-to-end web deployment model: static client distribution paired with containerized backend APIs running on ECS Fargate behind an Application Load Balancer.</li><li>Evaluated secure runtime configuration injection (database connection strings, JWT signing keys) into ECS tasks via AWS Secrets Manager.</li></ul> | Oct 02, 2026 | Oct 02, 2026 | [AWS Skill Builder — Module 3](https://skillbuilder.aws/renderer/?module_id=D18S53TDBA%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — AWS Lambda<br>03 — Containers and Orchestration on AWS<br>04 — Additional Compute Services |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

This week provided practical insights into containerization with Docker, Amazon ECR, and Amazon ECS Fargate. Previously, I ran our ASP.NET Core backend locally through the dotnet CLI; this module illustrated how the entire runtime is containerized, pushed to ECR, and orchestrated serverlessly via ECS Fargate without managing individual EC2 instances.

The serverless nature of Fargate—provisioning exact CPU and memory allocations per container—offered a direct solution for optimizing our operational budget during sprint verification and team demonstrations.

### Week 3 Learning Outcomes

- Serverless and containers represent leading cloud paradigms that accelerate release velocity while driving down idle infrastructure expenses.
- AWS Fargate eliminates virtual machine maintenance overhead, enabling engineering teams to focus solely on core application logic.
- Application in Tindy: Grasped packaging the ASP.NET Core backend into ECR Docker images and running serverless containers via ECS Fargate.
