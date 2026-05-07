---
title: NHTSA Vehicle Data Platform
date: 2026-05-03
summary: API-driven vehicle safety workflow for ingestion, medallion-style modeling, relational storage, and dashboard-ready recall analytics.
tags:
  - Python
  - APIs
  - Data Engineering
  - Analytics Platforms
  - PostgreSQL
---

API-driven vehicle safety data project focused on turning NHTSA public recall data into repeatable, dashboard-ready analytical outputs.

<!--more-->

The project is scoped around practical data engineering work: ingesting recall records from the public API, shaping them into medallion-style analytical tables, and preparing relational outputs for trend, manufacturer, component, and campaign-level reporting.

<div class="project-action-row">
  <a class="project-action" href="https://github.com/neibaur/portfolio-NHTSA" target="_blank" rel="noopener">View GitHub Repository</a>
</div>

<div class="project-tech-list">
  <span>Python</span>
  <span>NHTSA API</span>
  <span>PostgreSQL</span>
  <span>Supabase</span>
  <span>ETL</span>
  <span>Medallion Modeling</span>
  <span>Power BI</span>
  <span>Data Engineering</span>
</div>

Current focus areas:

- NHTSA public recall API ingestion
- Repeatable cleaning and normalization of recall records
- Medallion-style modeling for analytical datasets
- PostgreSQL/Supabase-ready relational structures
- Dashboard-ready outputs for recall, manufacturer, component, and campaign analysis
- Documentation of data design decisions during the 100DayDash challenge

Design notes:

- API ingestion and transformation are separated so raw records can be preserved while modeled tables evolve.
- Medallion-style layers provide a clear path from raw recall data to curated analytical outputs.
- Relational structures support dashboard tools without locking the project to one BI platform.
- Documentation captures tradeoffs and implementation decisions as the project matures.
