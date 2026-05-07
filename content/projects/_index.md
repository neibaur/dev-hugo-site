---
title: 'Projects'
date: 2024-05-19
type: landing

design:
  # Section spacing
  spacing: '3rem'

# Page sections
sections:
  - block: markdown
    content:
      title: Current Engineering Focus
      text: |
        <div class="projects-focus-list">
          <div>
            <strong>Cloud Automation & IaC:</strong>
            <span>Cloudflare governance, Terraform workflows, scheduled audits, secure secret handling, and optional remediation.</span>
          </div>
          <div>
            <strong>DevSecOps & Governance:</strong>
            <span>Dependabot, CodeQL, secret scanning, branch protection, automated validation, and CI/CD quality gates.</span>
          </div>
          <div>
            <strong>Data Engineering & APIs:</strong>
            <span>API ingestion, ETL pipelines, medallion-style modeling, Supabase/PostgreSQL, and dashboard-ready outputs.</span>
          </div>
          <div>
            <strong>Public Technical Documentation:</strong>
            <span>100DayDash notes covering platform engineering, cloud infrastructure, automation, analytics, and delivery tradeoffs.</span>
          </div>
        </div>
    design:
      css_class: "wide-block projects-focus"

  - block: collection
    content:
      title: Selected Projects
      text:
      filters:
        folders:
          - projects
    design:
      view: article-grid
      fill_image: false
      columns: 3
      show_date: false
      show_read_time: false
      show_read_more: false
      css_class: "projects-selected"
---
