---
title: "Workshop"
date: 2026-11-18
weight: 5
chapter: false
pre: " <b> 5. </b> "
---

Redeploy **Tindy on AWS using CloudFormation**, create a Fresh PostgreSQL database, run migrations and demo seeding, and verify the application through CloudFront before recording a web demonstration.

The workshop uses six templates, `foundation.yaml`, `network.yaml`, `database.yaml`, `integrations.yaml`, `runtime.yaml` and `edge.yaml`. Each deployment section explains resources, parameters, outputs required by subsequent stacks and verification results, with screenshots captured during execution.

## Agreed structure

| Section | Content |
| --- | --- |
| [5.1 Architecture overview](5.1-Overview/) | Tindy architecture, six templates and objectives. |
| [5.2 Deployment prerequisites](5.2-Prerequisites/) | AWS, CLI, source, image and mappings. |
| [5.3 Foundation and Network](5.3-Foundation-Network/) | Import Foundation and deploy networking. |
| [5.4 Database and Integrations](5.4-Database-Integrations/) | Fresh Database and PDF scanning integration. |
| [5.5 Runtime, seeding and Edge](5.5-Runtime-Edge/) | Edge maintenance, Runtime, bootstrap, migrations, seeding and live traffic. |
| [5.6 Application verification and demo video](5.6-Application-Demo/) | Demo video, onboarding, projects, matching, chat and AI PDF. |
| [5.7 Clean up resources](5.7-Cleanup/) | Recorded cleanup with verified progress and screenshots. |

## Current practical session

Tindy already exists, so this session starts with cleanup, documented in section 5.7. Redeployment recreates six stacks in the same environment, selects a Fresh database, seeds demo data and uses a new CloudFront hostname.

Recorded evidence covers maintenance and successful all six stacks, Runtime, Database, Integrations, Edge, Network and Foundation, all verified as DELETE_COMPLETE. Section 5.7 contains the detailed procedure and screenshots.
