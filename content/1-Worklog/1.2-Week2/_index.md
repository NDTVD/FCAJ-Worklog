---
title: "Week 2 Worklog"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

**Module 2** — Compute Services (EC2), Elastic Load Balancing (ELB), and Asynchronous Messaging

### Week 2 Objectives

- Evaluate Amazon EC2 instance families (General Purpose, Compute, Memory, Storage Optimized) matching specific application workload demands.
- Understand how Application Load Balancers (ALB), Auto Scaling Groups, and health checks maintain steady application availability.
- Grasp decoupling architectures utilizing Amazon Simple Queue Service (SQS) message queues and Amazon Simple Notification Service (SNS) pub/sub.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **EC2 Instance Families & Virtual Machine Lifecycle**<ul><li>Investigated hardware virtualization principles. Categorized instance families: T/M for general workloads, C for compute intensive, R for in-memory caching, and I/D for storage throughput.</li><li>Analyzed EC2 lifecycle states: Pending, Running, Stopping, Stopped, and Terminated. Evaluated billing implications regarding attached EBS volumes and public IP reallocations during stopped states.</li></ul> | Sep 21, 2026 | Sep 21, 2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Amazon EC2<br>02 — Amazon EC2 Instance Types |
| Tuesday | **EC2 Provisioning Mechanics & User Data Automation**<ul><li>Studied provisioning workflows via Console, CLI, and SDKs. Examined the roles of AMIs, SSH Key Pairs, and Security Group firewall port mappings (Port 80/443).</li><li>Evaluated bootstrap automation using User Data shell scripts to install runtime dependencies, configure web servers, and pull code upon initial launch.</li></ul> | Sep 22, 2026 | Sep 22, 2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — How to Provision AWS Resources<br>04 — Demo Launching an Amazon EC2 Instance |
| Wednesday | **Comparative Analysis of EC2 Purchasing Options**<ul><li>Contrasted five pricing tiers: On-Demand (maximum flexibility, billed per second), Savings Plans / Reserved Instances (1-3 year commitments saving up to 72%), Spot Instances (utilizing spare capacity with up to 90% discounts for fault-tolerant tasks), and Dedicated Hosts.</li><li>Formulated an economic selection matrix matching development testing against continuous production services.</li></ul> | Sep 23, 2026 | Sep 23, 2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Amazon EC2 Pricing |
| Thursday | **Horizontal Scaling & Elastic Load Balancing**<ul><li>Distinguished vertical scaling (scaling up) from horizontal elasticity (scaling out). Explored how Auto Scaling Groups dynamically provision instances triggered by CloudWatch alarms.</li><li>Analyzed Application Load Balancer mechanics: evaluating path-based request routing, native WebSocket protocol upgrades, and periodic Health Check probing to remove unhealthy targets.</li></ul> | Sep 24, 2026 | Sep 24, 2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Scaling Amazon EC2<br>07 — Directing Traffic with Elastic Load Balancing |
| Friday | **Asynchronous Decoupling via SQS & SNS**<ul><li>Explored publish/subscribe fanout patterns pairing Amazon SNS with Amazon SQS queues. Analyzed how loose coupling prevents cascading failures under burst traffic.</li><li>Compared SQS Standard Queues (unlimited throughput, at-least-once delivery) with SQS FIFO Queues (strict ordering, exactly-once processing) in file ingestion pipelines.</li></ul> | Sep 25, 2026 | Sep 25, 2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>08 — Messaging and Queuing |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

During this week on Compute and Messaging, I paid special attention to how Elastic Load Balancing (ALB) routes dynamic traffic. As the frontend engineer implementing real-time chat in Tindy, I recognized that ALBs do not merely distribute HTTP requests—they must support persistent WebSocket tunnels so users do not drop SignalR connections during live conversations.

Additionally, exploring Amazon SQS and SNS introduced me to asynchronous decoupling patterns. Rather than forcing the client interface into a blocking loader while scanning and parsing a large PDF resume, the backend can acknowledge receipt immediately and offload compute-intensive tasks to background queues, drastically improving client-side perceived responsiveness.

### Week 2 Learning Outcomes

- Matching instance families and purchasing models to actual workload profiles yields optimal cost-performance ratios.
- Pairing Application Load Balancers with Auto Scaling Groups provides autonomous resilience and traffic distribution.
- Application in Tindy: Learned how the Application Load Balancer (ALB) distributes traffic and maintains persistent WebSocket connections for two-way SignalR chat.
