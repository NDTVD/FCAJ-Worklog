---
title: "Week 5 Worklog"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

**Module 5** — Amazon VPC, network security, and global networking

### Week 5 Objectives

- Trace traffic through a VPC, subnets, and route tables.
- Distinguish security groups from network ACLs and select connectivity by use case.
- Explain the roles of Route 53, CloudFront, and Global Accelerator in global networking.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **VPC and network boundaries**<ul><li>Review connectivity needs for AWS resources, branch networks, and remote users. Analyze the scope of a VPC and the roles of an internet gateway and a virtual private gateway.</li><li>Draw the VPC as the application's network boundary and add paths to the internet, a branch network, and remote users. Explain which path uses an internet gateway and where a virtual private gateway fits in private connectivity.</li></ul> | Oct 12, 2026 | Oct 12, 2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Networking<br>02 — Organizing AWS Cloud Resources |
| Tuesday | **Connectivity for users, networks, and services**<ul><li>Compare AWS Client VPN, AWS Site-to-Site VPN, AWS Direct Connect, and AWS PrivateLink by use case.</li><li>Use scenarios for remote staff, office connectivity, dedicated links, and private access to a service. Choose Client VPN, Site-to-Site VPN, Direct Connect, or PrivateLink for each and explain the connection scope.</li></ul> | Oct 13, 2026 | Oct 13, 2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — More Ways to Connect to the AWS Cloud |
| Wednesday | **Subnets, routing, and traffic controls**<ul><li>Compare public and private subnets, stateful security groups, and stateless network ACLs. Review the VPC demo with public and private subnets across two AZs, an internet gateway, and a route table.</li><li>Trace a request to a server in a VPC with public and private subnets across two AZs. Read the route table, then check both filtering layers: security groups track connection state, while network ACLs require reviewing rules in both directions.</li></ul> | Oct 14, 2026 | Oct 14, 2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Subnets, Security Groups, and Network Access Control Lists<br>05 — Amazon VPC Demo |
| Thursday | **DNS, content delivery, and traffic acceleration**<ul><li>Distinguish DNS through Route 53, content delivery through CloudFront, and traffic acceleration through Global Accelerator.</li><li>Use an application with a custom domain and static content to distinguish name resolution from content delivery. Annotate Route 53, CloudFront, and Global Accelerator at their respective points in the diagram.</li></ul> | Oct 15, 2026 | Oct 15, 2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Global Networking |
| Friday | **Redundant connectivity and global delivery**<ul><li>Review example architectures for resilient Direct Connect connectivity and content delivery across Regions.</li><li>Review two cases: redundant Direct Connect connectivity and content delivery across Regions. Identify what needs redundancy in each case and sketch what happens when a connection or destination becomes unavailable.</li></ul> | Oct 16, 2026 | Oct 16, 2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>07 — Global Architectures |

### Week 5 Learning Outcomes

- Client VPN connects remote users, Site-to-Site VPN connects networks, Direct Connect provides dedicated connectivity, and PrivateLink enables private access to services.
- Route tables determine traffic paths in a VPC. For global users, Route 53 handles DNS, CloudFront delivers content, and Global Accelerator optimizes traffic paths.
- **Application in Tindy:** Understood VPC segmentation with Private Database Subnets and configuring CloudFront VPC Origins to reach the internal ALB.

