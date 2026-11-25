---
title: "Week 8 Worklog"
date: 2024-01-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

**Module 8** — AI, machine learning, and data analytics

### Week 8 Objectives

- Distinguish training, inference, and the levels of the AWS AI/ML stack.
- Choose generative AI tools based on application and team needs.
- Explain how a pipeline moves data from its source to storage, analytics, and model training.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **AI/ML and the AWS service tiers**<ul><li>Follow data from preparation through training and inference. Use product recommendations to distinguish hand-written rules from a model trained on data.</li><li>Group the AWS options into prebuilt AI services, Amazon SageMaker AI, and frameworks on team-managed infrastructure. Explain the trade-off between integration time and control.</li></ul> | Nov 2, 2026 | Nov 2, 2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to AI and Machine Learning<br>02 — AI-ML on AWS |
| Tuesday | **Selecting AI/ML services by use case**<ul><li>Compare Amazon Polly for text-to-speech with Amazon Comprehend for language analysis. For each case, identify the input and the output the backend would use.</li><li>Compare using a prebuilt service with building a custom model on SageMaker AI. Identify the training data, evaluation criteria, and operational responsibilities before choosing.</li></ul> | Nov 3, 2026 | Nov 3, 2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — AWS AI-ML Solutions |
| Wednesday | **Foundation models and generative AI**<ul><li>Distinguish foundation models from LLMs and compare Amazon Bedrock, SageMaker JumpStart, Amazon Q Business, and Amazon Q Developer in the lesson scenarios.</li><li>Relate Tindy's profile draft workflow to Bedrock. Identify the input, structured output, and user review step. Review how RAG retrieves relevant context for the model request.</li></ul> | Nov 4, 2026 | Nov 4, 2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Introduction to Generative AI on AWS<br>05 — AWS Generative AI Solutions |
| Thursday | **From data sources to reports**<ul><li>Distinguish an S3 data lake from a data warehouse and compare ETL, ELT, and Zero-ETL approaches using the study notes.</li><li>Sketch ingestion with Kinesis Data Streams or Data Firehose, cataloging and processing with Glue or EMR, querying through Athena or Redshift, and visualization. Identify data quality issues to address before reporting.</li></ul> | Nov 5, 2026 | Nov 5, 2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Introduction to Data Analytics<br>07 — Data Pipelines on AWS |
| Friday | **Combining data analytics and ML**<ul><li>Trace the example DynamoDB changes through Kinesis Data Streams and Data Firehose. Mark the Lambda transformation and the long-term storage in S3.</li><li>Separate the two uses after data reaches the lake. Athena uses Glue Data Catalog metadata for queries, while SageMaker AI uses suitable data for training. Note how to check data consistency for both paths.</li></ul> | Nov 6, 2026 | Nov 6, 2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>08 — Data Analytics and AI-ML |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

This was one of the most exciting modules, tying directly into Tindy's flagship generative AI capability: CV parsing and intelligent recommendation via Amazon Bedrock.

I learned that production AI applications should combine deterministic business rules with semantic embeddings rather than relying solely on raw LLM inferences. On the frontend, I translated this into the AI Draft Review UI: when Bedrock parses resume skills, the interface renders editable tag chips so students can verify, modify, or reject suggestions before committing data to PostgreSQL.

### Week 8 Learning Outcomes

- Prebuilt AI services, managed model development, and self-managed infrastructure serve different needs.
- Generative AI output needs application-specific validation before it enters profiles or business workflows.
- A data lake can serve analytics and ML when data is processed, cataloged, and checked for quality.
- **Application in Tindy:** Integrated Amazon Bedrock for CV skill parsing; engineered the AI Draft Review UI allowing candidates to review and edit suggestions.


