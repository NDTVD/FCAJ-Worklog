---
title: "Week 13 Worklog"
date: 2024-01-01
weight: 13
chapter: false
pre: " <b> 1.13. </b> "
---

**Module 13** — AWS Well-Architected and internship wrap-up

### Week 13 Objectives

- Apply the six pillars of the AWS Well-Architected Framework to a workload review.
- Explain when to use specialized AWS services through the course architecture examples.
- Relate Tindy's architectural trade-offs to the course and prepare the internship wrap-up materials.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **From a working system to an architecture review**<ul><li>Read the Tindy diagram and group its components into the CloudFront entry point, ECS Fargate compute, PostgreSQL database, and S3 document flow.</li><li>Ask about recovery, security, and operations at each layer. Use the demo configuration to document assumptions about users, runtime, and acceptable downtime.</li></ul> | Dec 7, 2026 | Dec 7, 2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Well-Architected Solutions |
| Tuesday | **Specialized AWS services**<ul><li>Match CodePipeline to CI/CD orchestration, X-Ray to distributed tracing, AppSync to GraphQL APIs, and Amplify to web application development.</li><li>Compare Amazon SES and Amazon Connect for email and contact center needs. Distinguish the lesson's examples of application streaming, managed desktops, and managed web access by what users need to do.</li></ul> | Dec 8, 2026 | Dec 8, 2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>02 — AWS Specialized Services |
| Wednesday | **The six AWS Well-Architected pillars**<ul><li>Build a table of the six pillars: Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization, and Sustainability. Map each pillar to one question for the application.</li><li>Distinguish the Framework's guidance from the Well-Architected Tool's review workflow. Consider how to prioritize risks by impact, record evidence, and identify follow-up checks.</li></ul> | Dec 9, 2026 | Dec 9, 2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — AWS Well-Architected Framework |
| Thursday | **Three specialized architecture use cases**<ul><li>Trace a request through a serverless backend using API Gateway, Lambda, and DynamoDB. Identify where logs and traces can help investigate errors or latency.</li><li>Compare this with an S3-hosted static site whose contact form sends email through SES and an Amazon Connect contact center with multiple channels or callback. Identify what each service handles.</li></ul> | Dec 10, 2026 | Dec 10, 2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Specialized Use Cases |
| Friday | **Reviewing Tindy and consolidating the course**<ul><li>Use the six pillars to review the Tindy demo. Compare the limitations of one Fargate task and Single-AZ RDS with readiness monitoring, backups, and recovery after a failure.</li><li>Distinguish what the code or documentation already describes from what still needs verification. Prepare a list of objectives, evidence, and references for the bilingual report.</li></ul> | Dec 11, 2026 | Dec 11, 2026 | [AWS Skill Builder — Module 13](https://skillbuilder.aws/renderer/?module_id=B4R4AU7BWJ%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to Well-Architected Solutions<br>03 — AWS Well-Architected Framework<br>04 — Specialized Use Cases |
| Monday | **Internship wrap-up**<ul><li>Complete the internship wrap-up and finalize the report.</li><li>Finalize the self-assessment based on the knowledge and work recorded. Review the table of contents, both language versions, and the source of each piece of evidence before finalizing the report.</li></ul> | Dec 14, 2026 | Dec 14, 2026 | Internship report |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

The final week offered an opportunity to evaluate our overall internship progress against the six pillars of the AWS Well-Architected Framework (Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization, Sustainability).

Reviewing Tindy through these architectural lenses ensured our frontend delivery, backend throttling, and infrastructure provisioning met rigorous standards, culminating in our successful Workshop Section 5.6 demonstration video. This internship strengthened both my core frontend engineering competencies and practical cloud architectural thinking.

### Week 13 Learning Outcomes

- The six pillars provide architecture review criteria. The Well-Architected Tool helps record answers, risks, and improvements.
- The roles of specialized services can be explained through three examples: a serverless backend, a contact form, and a contact center.
- The wrap-up relates Tindy's demo context to security, reliability, operations, and cost decisions.
- **Application in Tindy:** Assessed Tindy against the 6 Well-Architected pillars; finalized end-to-end UI verification and Workshop Section 5.6 demo scenarios.


