---
title: 'Projects'
date: 2024-05-19
type: landing

design:
  # Section spacing
  spacing: '5rem'

# Page sections
sections:
  - block: markdown
    content:
      title: Current Engineering Focus
      text: |
        - Cloudflare governance and remediation platform using Terraform, GitHub Actions, and Python
        - Public 100-day engineering initiative documenting cloud infrastructure and data platform development
        - NHTSA analytics platform using API ingestion, medallion-style architecture, Supabase, and Power BI
        - DevSecOps workflows with CodeQL, Dependabot, automated validation, and CI/CD governance
        - Dashboard engineering projects using Power BI, Looker Studio, Astro, Hugo, and Python visualization tools
    design:
      css_class: "wide-block"

  - block: collection
    content:
      title: Selected Projects
      text: A focused collection of recent portfolio projects and in-progress case studies demonstrating data engineering, dashboard development, automation, and cloud-integrated analytics. In-progress projects are included when they show real implementation progress.
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
---
