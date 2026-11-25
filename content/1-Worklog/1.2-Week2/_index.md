---
title: "Week 2 Worklog"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

**Module 2** — EC2, traffic distribution, and messaging

### Week 2 Objectives

- Choose an Amazon EC2 instance type and provisioning method based on workload requirements.
- Compare EC2 purchasing options and explain the roles of Auto Scaling, Elastic Load Balancing, and health checks.
- Explain how Amazon SQS and Amazon SNS decouple application components.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **EC2 instance lifecycle and categories**<ul><li>Review virtualization and EC2 instance lifecycle states. Compare instance categories by CPU, memory, hardware acceleration, and storage requirements.</li><li>Record the operating system, compute capacity, and storage choices available when provisioning EC2. Compare stopping and terminating an instance, then map instance categories to a typical web backend, a CPU-intensive job, and a memory-intensive workload.</li></ul> | Sep 21, 2026 | Sep 21, 2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Amazon EC2<br>02 — Amazon EC2 Instance Types |
| Tuesday | **Provisioning tools and the EC2 launch demo**<ul><li>Compare the AWS Management Console, AWS CLI, CloudShell, and AWS SDKs for provisioning and managing resources. Review the EC2 web server launch demo, including the AMI, key pair, network settings, EBS, and user data.</li><li>Compare viewing EC2 information through the console, CLI, and SDK to explain when each tool fits. Trace the launch demo and annotate which settings govern initial software, access, networking, storage, and startup configuration.</li></ul> | Sep 22, 2026 | Sep 22, 2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — How to Provision AWS Resources<br>04 — Demo Launching an Amazon EC2 Instance |
| Wednesday | **Amazon EC2 pricing**<ul><li>Compare On-Demand, Savings Plans, Reserved Instances, Spot Instances, and Dedicated Hosts against workload needs.</li><li>Build a decision table covering short experiments, steady workloads, interruptible jobs, and software with physical-host requirements. For each case, explain the purchasing option and the constraint to check first.</li></ul> | Sep 23, 2026 | Sep 23, 2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — Amazon EC2 Pricing |
| Thursday | **Scaling and load balancing**<ul><li>Distinguish vertical and horizontal scaling. Review Auto Scaling groups and the role of CloudWatch. Analyze how Elastic Load Balancing distributes traffic and uses health checks.</li><li>Explain how an application handles a traffic spike. EC2 Auto Scaling adjusts group capacity while the load balancer routes requests to healthy targets. Diagram what happens when a target fails and show where health checks fit.</li></ul> | Sep 24, 2026 | Sep 24, 2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Scaling Amazon EC2<br>07 — Directing Traffic with Elastic Load Balancing |
| Friday | **Queuing, notifications, and fanout**<ul><li>Compare Amazon SQS queues and Amazon SNS publish/subscribe through a fanout example.</li><li>Describe a producer placing an image-processing request on a queue and a worker consuming it. Extend the example into fanout so one event reaches multiple queues, each with a separate consumer task. Explain where SNS and SQS fit.</li></ul> | Sep 25, 2026 | Sep 25, 2026 | [AWS Skill Builder — Module 2](https://skillbuilder.aws/renderer/?module_id=422P3V2XSR%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>08 — Messaging and Queuing |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

During this week on Compute and Messaging, I paid special attention to how Elastic Load Balancing (ALB) routes dynamic traffic. As the frontend engineer implementing real-time chat in Tindy, I recognized that ALBs do not merely distribute HTTP requests—they must support persistent WebSocket tunnels so users do not drop SignalR connections during live conversations.

Additionally, exploring Amazon SQS and SNS introduced me to asynchronous decoupling patterns. Rather than forcing the client interface into a blocking loader while scanning and parsing a large PDF resume, the backend can acknowledge receipt immediately and offload compute-intensive tasks to background queues, drastically improving client-side perceived responsiveness.

### Week 2 Learning Outcomes

- Instance selection depends on workload requirements. The AMI specifies the initial software, and user data can run configuration steps at launch.
- EC2 Auto Scaling adjusts instance count, Elastic Load Balancing distributes requests, and SQS and SNS support asynchronous communication.
- **Application in Tindy:** Learned how the Application Load Balancer (ALB) distributes traffic and maintains persistent WebSocket connections for two-way SignalR chat.


