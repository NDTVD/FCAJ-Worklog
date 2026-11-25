---
title: "Week 7 Worklog"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

**Module 7** — AWS databases and in-memory caching

### Week 7 Objectives

- Choose a relational or NoSQL database based on data relationships, transactions, and access patterns.
- Analyze the SQL and DynamoDB operations in the course demonstration.
- Explain the roles of caching, purpose-built databases, and backups.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **Choosing a database for the workload**<ul><li>Use a coffee shop loyalty program to identify the customer, purchase, and points records that need to be stored.</li><li>List common reads and writes before selecting a service. Relate this to the connections among accounts, projects, and applications in Tindy, and explain how access patterns shape the data model.</li></ul> | Oct 26, 2026 | Oct 26, 2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Databases |
| Tuesday | **SQL, Amazon RDS, and Amazon Aurora**<ul><li>Review tables, primary and foreign keys, and SQL transactions. Use a recruitment update to explain why several related changes must stay consistent.</li><li>Compare self-managed databases on EC2 with Amazon RDS and Aurora. Identify remaining application responsibilities, including schema and access control, and review how backups and point-in-time recovery support operations.</li></ul> | Oct 27, 2026 | Oct 27, 2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — Relational Database Services |
| Wednesday | **Amazon DynamoDB and NoSQL access patterns**<ul><li>Distinguish tables, items, and attributes. Identify the partition key and decide when a sort key is useful for storing multiple items under it.</li><li>Outline how the chosen key supports listing a customer's orders. Compare single-Region access with a workload that needs reads and writes in multiple Regions to understand the role of DynamoDB Global Tables.</li></ul> | Oct 28, 2026 | Oct 28, 2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — NoSQL Database Services |
| Thursday | **Reviewing the RDS and DynamoDB demonstration**<ul><li>Follow the RDS MySQL demo from database and table creation through inserting rows and using JOIN to read related records.</li><li>Compare this with the DynamoDB demo that creates a table and adds items through the SDK. Contrast a key-based Query with a table Scan and explain how that affects the amount of data read. Note the resources to check if repeating the demo.</li></ul> | Oct 29, 2026 | Oct 29, 2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — AWS Databases Demonstration |
| Friday | **Caching and purpose-built databases**<ul><li>Diagram cache hits and misses between the API, ElastiCache, and RDS. Consider cache lifetime and the risk of serving stale data after an update.</li><li>Match DocumentDB to document data, Neptune to graph relationships, DAX to accelerating DynamoDB reads, and Managed Blockchain to a distributed ledger use case. Relate AWS Backup to recovery from a backup point.</li></ul> | Oct 30, 2026 | Oct 30, 2026 | [AWS Skill Builder — Module 7](https://skillbuilder.aws/renderer/?module_id=B1DGAV8S16%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>05 — In-Memory Caching Services<br>06 — Additional Database Services |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

Module 7 contrasted relational databases (Amazon RDS PostgreSQL) with NoSQL architectures (Amazon DynamoDB). For Tindy, PostgreSQL proved optimal due to heavily normalized business logic: Users mapped to Profiles, Projects containing multiple Position entities, and Applications binding applicants to seats.

Understanding relational queries and foreign key constraints helped me design clean TypeScript interfaces that mirror backend DTO payloads accurately during API integration.

### Week 7 Learning Outcomes

- Query patterns, relationships, and transaction requirements guide service and key design.
- The course demo illustrates the difference between RDS JOIN operations and DynamoDB Query and Scan.
- Caching reduces direct database reads. Backup policies and recovery checks address data protection.
- **Application in Tindy:** Studied the relational schema in RDS PostgreSQL 17 for Profiles, Projects, Match criteria, and chat history.


