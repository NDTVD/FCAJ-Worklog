---
title: "Week 8 Worklog"
date: 2024-01-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

**Module 8** — Artificial Intelligence (AI/ML), Amazon Bedrock, and Intelligent Resume Extraction

### Week 8 Objectives

- Survey AWS AI/ML services and differentiate Generative AI capabilities from classical predictive machine learning models.
- Understand Amazon Bedrock's serverless foundation model APIs and evaluate model families such as Anthropic Claude 3 Sonnet and Haiku.
- Master Prompt Engineering techniques to reliably extract structured JSON from raw PDF resumes and visualize suggestions within React UI.

### Tasks for the Week

| Day | Task | Start Date | Completion Date | References |
| --- | --- | --- | --- | --- |
| Monday | **AWS AI/ML Ecosystem & Generative AI Paradigms**<ul><li>Surveyed the AWS AI stack: application layer services (Rekognition, Textract), machine learning platforms (SageMaker), and serverless Generative AI (Amazon Bedrock).</li><li>Evaluated Generative AI capabilities for talent matchmaking: extracting domain context from unstructured student resumes to propose tailored project opportunities.</li></ul> | Nov 02, 2026 | Nov 02, 2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>01 — Introduction to AI and Machine Learning<br>02 — AI-ML on AWS |
| Tuesday | **Amazon Bedrock & Foundation Model Ecosystems**<ul><li>Investigated Amazon Bedrock: a fully managed service offering unified API access to leading foundation models from Anthropic, Meta, and Amazon without infrastructure management.</li><li>Evaluated Anthropic Claude model variants: lightweight Haiku for low-latency tasks versus Sonnet for balanced semantic parsing; analyzed temperature and top_p hyperparameter tuning.</li></ul> | Nov 03, 2026 | Nov 03, 2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>03 — AWS AI-ML Solutions |
| Wednesday | **Prompt Engineering & Structured JSON Output Schemas**<ul><li>Studied prompt engineering methodologies: persona framing, contextual grounding, and few-shot examples enforcing deterministic output syntax.</li><li>Authored parsing prompts instructing foundation models to extract structured JSON (technical skills, work experience, bio) from extracted PDF text while suppressing extraneous commentary.</li></ul> | Nov 04, 2026 | Nov 04, 2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>04 — Introduction to Generative AI on AWS<br>05 — AWS Generative AI Solutions |
| Thursday | **AI Studio UI Implementation & Human-in-the-Loop UX**<ul><li>Engineered the AI Studio view in React: providing intuitive PDF file pickers, animated scanning indicators, and interactive suggestion chip components.</li><li>Implemented a human-in-the-loop workflow: allowing students to review, edit, or reject AI-extracted skills before committing them to their profile records.</li></ul> | Nov 05, 2026 | Nov 05, 2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>06 — Introduction to Data Analytics<br>07 — Data Pipelines on AWS |
| Friday | **Token Optimization Economics & Responsible AI Safeguards**<ul><li>Analyzed Amazon Bedrock billing formulas tied to input/output token counts; developed prompt trimming routines to prune whitespace and reduce API expenses.</li><li>Reviewed AWS Responsible AI principles: ensuring candidate resume data remains strictly isolated in private customer VPCs and is never used to train public foundation models.</li></ul> | Nov 06, 2026 | Nov 06, 2026 | [AWS Skill Builder — Module 8](https://skillbuilder.aws/renderer/?module_id=NUYARVB13G%3A002.000.000&product_id=8D79F3AVR7%3A003.002.003&registration_id=a5d67877-3d77-5f7a-9e56-2ddce1349824&referrer=https%3A%2F%2Fskillbuilder.aws%2Flearn%2F94T2BEN85A%2Faws-cloud-practitioner-essentials%2F8D79F3AVR7&navigation=digital)<br>08 — Data Analytics and AI-ML |

### Personal Reflections & Frontend Perspective (Cao Thành Nhân)

Week 8's dive into Amazon Bedrock and Generative AI proved to be one of the most rewarding milestones. Engineering the AI Studio interface in Tindy demanded tight integration between client-side UX state machines and cloud foundation model APIs.

Because generative model parsing typically takes 3–6 seconds, silent blocking loaders degrade user confidence. I designed an interactive resume scanner animation accompanied by multi-step status milestones. Presenting AI suggestions as clickable badge chips gave students complete autonomy to accept or prune parsed skills before committing changes to their database records.

### Week 8 Learning Outcomes

- Amazon Bedrock unlocks enterprise-grade Generative AI integrations via unified APIs without GPU hardware management overhead.
- Precise prompt engineering paired with strict JSON output schemas enables reliable structured data extraction from unstructured resumes.
- Application in Tindy: Built the React AI Studio screen; supported CV PDF uploads and interactive selection of Bedrock-extracted skills.
