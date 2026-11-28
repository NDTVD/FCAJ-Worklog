---
title: "Week 1 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

**Module 1** — Cloud Computing Fundamentals and AWS Global Infrastructure

### Week 1 Objectives

- Master the fundamentals of the Client-Server architecture, on-demand pay-as-you-go billing, and the shift from on-premises hardware to cloud infrastructure.
- Analyze the hierarchical structure of AWS Global Infrastructure: Regions, Availability Zones (AZs), and edge locations to optimize deployment locality.
- Understand the AWS Shared Responsibility Model to clearly demarcate security boundaries between the cloud provider and application developers.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Cloud Computing Principles & Client-Server Mechanics**<ul><li>Explored client-server interaction: web browsers acting as clients dispatching HTTP requests across the network to receive generated server payloads.</li><li>Contrasted capital expenditure (CAPEX) in physical data centers with variable operational expenditure (OPEX) in the cloud. Analyzed how elasticity eliminates idle compute overhead.</li></ul> | Sep 14, 2026 | Sep 14, 2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01–02 — Welcome to AWS Cloud Practitioner Essentials<br>What is Cloud Computing |
| Tuesday | **Deep Dive into the Six Advantages of Cloud Computing**<ul><li>Evaluated the six core cloud benefits: trade capital expense for variable expense, benefit from massive economies of scale, stop guessing capacity, increase speed and agility, stop spending money running data centers, and go global in minutes.</li><li>Modeled these advantages against real-world scenarios for student project recruitment workloads during peak registration periods.</li></ul> | Sep 15, 2026 | Sep 15, 2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — Benefits of the AWS Cloud |
| Wednesday | **AWS Global Infrastructure Breakdown**<ul><li>Investigated Regions and Availability Zones. Every AWS Region contains multiple isolated AZs with independent power, cooling, and low-latency fiber connectivity.</li><li>Analyzed resilient Multi-AZ architecture patterns: validating how automated failover safeguards web availability when an individual data center experiences outages.</li></ul> | Sep 16, 2026 | Sep 16, 2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Introduction to AWS Global Infrastructure |
| Thursday | **AWS Shared Responsibility Model Demarcation**<ul><li>Studied security boundaries: AWS secures the underlying cloud infrastructure (hardware, hypervisors, facilities), while users are strictly responsible for guest OS configurations, data encryption, IAM policies, and application codebase.</li><li>Contrasted operational management scope across unmanaged infrastructure (EC2) versus managed services (RDS, S3).</li></ul> | Sep 17, 2026 | Sep 17, 2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — The AWS Shared Responsibility Model |
| Friday | **Web Application Cloud Architecture Case Study**<ul><li>Designed a conceptual deployment layout for a web platform serving regional students. Assessed Region selection criteria balancing user round-trip latency against regional pricing differences.</li><li>Drafted structural separation separating client static bundles from dynamic API endpoints across redundant Availability Zones.</li></ul> | Sep 18, 2026 | Sep 18, 2026 | [AWS Skill Builder — Module 1](https://skillbuilder.aws/renderer/?module_id=ZWYR2AX7VG%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Applying Cloud Concepts to Real Life Use Cases |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

As a frontend developer focused on React and TypeScript, I previously viewed web applications strictly through the browser runtime: state trees, component lifecycles, and UI styling. Week 1 broadened my engineering horizon by connecting browser execution to the global cloud infrastructure that supports it.

Studying the Client-Server paradigm and AWS Global Infrastructure clarified how network packets travel from client viewports to cloud compute endpoints. The Shared Responsibility Model served as a vital takeaway: safeguarding client-side data, preventing credential leakage in public JavaScript bundles, and enforcing secure CORS origins are developer obligations that AWS cannot manage on our behalf.

### Week 1 Learning Outcomes

- Cloud elasticity shifts capital expenditure into variable operating expense, freeing engineering teams from physical hardware maintenance.
- Multi-AZ architecture represents a foundational best practice for continuous web application availability.
- Application in Tindy: Analyzed the Client–Server interaction between the React frontend (Vite) and ASP.NET Core API; studied on-demand pricing models to manage costs for demo resources.
