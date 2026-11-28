---
title: "Week 5 Worklog"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

**Module 5** — Cloud Networking (Amazon VPC), Routing, and API Connectivity

### Week 5 Objectives

- Design isolated virtual network architectures using Amazon VPC CIDR blocks, segregating Public and Private Subnets securely.
- Differentiate operational flows across Internet Gateways, NAT Gateways, and Route Tables for inbound and outbound traffic control.
- Master multi-layered network security with Security Groups, Network ACLs, and implement robust Cross-Origin Resource Sharing (CORS) policies.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Amazon VPC Design & Subnet Segmentation**<ul><li>Investigated isolated cloud networking with Amazon VPC CIDR allocations (e.g., /16 for VPC and /24 for subnets).</li><li>Designed a multi-tier network topology: deploying public-facing Application Load Balancers in Public Subnets, while isolating ECS Fargate tasks and RDS PostgreSQL databases in Private Subnets without public IPs.</li></ul> | Oct 12, 2026 | Oct 12, 2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Networking<br>02 — Organizing AWS Cloud Resources |
| Tuesday | **Internet Gateways, NAT Gateways & Route Tables**<ul><li>Examined Internet Gateways facilitating bidirectional HTTP/HTTPS internet communication for public subnets.</li><li>Analyzed NAT Gateways deployed in public subnets: granting egress internet access for private ECS tasks (fetching NuGet packages, invoking Amazon Bedrock) while dropping unprompted inbound connections.</li></ul> | Oct 13, 2026 | Oct 13, 2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — More Ways to Connect to the AWS Cloud |
| Wednesday | **Network Defense Layers: Security Groups vs NACLs**<ul><li>Contrasted Stateful Security Groups (instance/task-level filtering) with Stateless Network ACLs (subnet-level subnet boundary filtering).</li><li>Formulated strict least-privilege firewall rules: chaining ECS security groups to only accept inbound HTTP traffic from ALB security groups, and restricting RDS PostgreSQL (port 5432) strictly to ECS tasks.</li></ul> | Oct 14, 2026 | Oct 14, 2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Subnets, Security Groups, and Network Access Control Lists<br>05 — Amazon VPC Demo |
| Thursday | **Cross-Origin Resource Sharing (CORS) & Browser Security**<ul><li>Analyzed CORS mechanics triggered when browser clients issue fetch requests from CloudFront frontend origins (`*.cloudfront.net`) to ALB backend API origins (`*.elb.amazonaws.com`).</li><li>Investigated browser preflight `OPTIONS` handshakes and enforced server-side response headers: `Access-Control-Allow-Origin`, `Access-Control-Allow-Headers`, and `Access-Control-Allow-Methods`.</li></ul> | Oct 15, 2026 | Oct 15, 2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Global Networking |
| Friday | **End-to-End Network Verification & Latency Profiling**<ul><li>Validated end-to-end routing paths using cURL and browser network inspection tools, ensuring proper HTTP 200 responses and header propagation.</li><li>Traced packet paths from client edge through CloudFront, traversing public ALB listeners into private ECS containers and secure database subnets.</li></ul> | Oct 16, 2026 | Oct 16, 2026 | [AWS Skill Builder — Module 5](https://skillbuilder.aws/renderer/?module_id=K457BUCF7F%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>07 — Global Architectures |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

As a frontend developer, the most persistent hurdle when connecting a React client to backend services is CORS (Cross-Origin Resource Sharing) restrictions. Week 5 demystified the underlying browser security mechanisms enforcing origin isolation.

Understanding browser Preflight OPTIONS handshakes and configuring proper CORS headers across network tiers empowered me to eliminate cross-origin blockers in Tindy. Furthermore, learning how private subnets shield database instances and internal APIs provided immense confidence in our application's production security posture.

### Week 5 Learning Outcomes

- Public/Private subnet isolation combined with NAT Gateways forms the standard defense blueprint for shielding internal backend services.
- Stateful Security Groups enforce strict least-privilege network communication between decoupled architectural tiers.
- Application in Tindy: Traced routing flows between CloudFront, ALB, and ECS; configured backend CORS policies to ensure seamless React API connectivity.
