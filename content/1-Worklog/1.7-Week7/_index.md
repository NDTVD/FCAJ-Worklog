---
title: "Week 7 Worklog"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

**Module 7** — Cloud Databases (RDS PostgreSQL, DynamoDB) and In-Memory Caching

### Week 7 Objectives

- Analyze architectural trade-offs between Relational Database Services (Amazon RDS) and non-relational NoSQL (Amazon DynamoDB).
- Understand high-availability database resiliency: Multi-AZ failover, Read Replicas scaling, and Automated Point-in-Time Recovery.
- Master frontend data consumption optimization: pagination patterns, client-side query caching, and UI skeleton loading states.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Relational Database Management with Amazon RDS PostgreSQL**<ul><li>Investigated Amazon Relational Database Service (RDS): automated provisioning, automated OS patching, point-in-time snapshots, and continuous backups.</li><li>Modeled Tindy's relational schema: Users, Projects, Applications, and Message tables bound by foreign keys enforcing strict ACID transactional integrity.</li></ul> | Oct 26, 2026 | Oct 26, 2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Databases |
| Tuesday | **RDS Multi-AZ High Availability & Read Replicas**<ul><li>Analyzed Multi-AZ synchronous replication: maintaining hot standby replicas across distinct AZs with automated DNS failover during hardware interruptions.</li><li>Explored Read Replicas: provisioning asynchronous read-only nodes to offload heavy read queries from project search filters and candidate browsing views.</li></ul> | Oct 27, 2026 | Oct 27, 2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — Relational Database Services |
| Wednesday | **NoSQL Scale with Amazon DynamoDB**<ul><li>Explored Amazon DynamoDB architectures: fully managed serverless key-value and document store delivering single-digit millisecond latency at any throughput scale.</li><li>Evaluated Partition Key (PK) and Sort Key (SK) indexing strategies for tracking real-time user presence, notifications, and event streams.</li></ul> | Oct 28, 2026 | Oct 28, 2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — NoSQL Database Services |
| Thursday | **In-Memory Caching via Amazon ElastiCache (Redis)**<ul><li>Studied Cache-Aside caching patterns: storing high-read, low-write lookup tables (skills taxonomies, featured project listings) in ultra-fast RAM caches.</li><li>Investigated Time-to-Live (TTL) expiration policies and cache invalidation hooks preventing stale data presentation across client viewports.</li></ul> | Oct 29, 2026 | Oct 29, 2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — AWS Databases Demonstration |
| Friday | **Frontend Data Ingestion, Pagination & UX Resilience**<ul><li>Compared pagination implementations: Offset/Limit vs Cursor-based streaming to protect browser memory from unbounded dataset ingestion.</li><li>Engineered client-side UI states in React: animated Skeleton loaders during asynchronous data fetches, graceful empty states, and database connection timeout alerts.</li></ul> | Oct 30, 2026 | Oct 30, 2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — In-Memory Caching Services<br>06 — Additional Database Services |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

Previously, I assumed database performance was solely an issue of backend SQL optimization. Week 7 revealed how drastically client-side consumption patterns impact underlying database stability.

If a React search input dispatches unthrottled API calls on every keystroke without input debouncing, or attempts to fetch 10,000 project records in a single unpaginated query, the database will quickly degrade. I implemented search input debouncing and paginated infinite scrolling within Tindy's discovery views to protect our PostgreSQL instance from redundant compute loads.

### Week 7 Learning Outcomes

- Amazon RDS PostgreSQL delivers rock-solid ACID reliability, while Multi-AZ failover protects core business records from hardware outages.
- Integrating in-memory caching and cursor pagination shields databases from unbounded traffic spikes.
- Application in Tindy: Built debounced search inputs and paginated data tables in React, eliminating redundant query loads on RDS PostgreSQL.
