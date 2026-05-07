---
title: 'Experience'
date: 2023-10-24
type: landing

design:
  spacing: '2rem'

# Note: `username` refers to the user's folder name in `content/authors/`

# Page sections
sections:
  - block: markdown
    content:
      title: ''
      text: |
        <h2 class="experience-section-title">Technical Stack</h2>

        <div class="experience-stack-list">
          <div>
            <strong>Languages & Automation</strong>
            <span>Python &middot; SQL &middot; REST APIs &middot; Postman &middot; Selenium</span>
          </div>
          <div>
            <strong>Cloud & Platform Engineering</strong>
            <span>Terraform &middot; GitHub Actions &middot; Docker &middot; Kubernetes &middot; Cloudflare &middot; CI/CD</span>
          </div>
          <div>
            <strong>Data & Analytics Platforms</strong>
            <span>Databricks &middot; PostgreSQL &middot; Supabase &middot; Power BI &middot; ETL Pipelines</span>
          </div>
          <div>
            <strong>Operational Tooling</strong>
            <span>Git &middot; Linux &middot; Jira &middot; ServiceNow &middot; Agile</span>
          </div>
        </div>
    design:
      css_class: "wide-block experience-stack"

  - block: work-experience
    content:
      username: me
    design:
      # Hugo date format
      date_format: 'January 2006'

  - block: markdown
    content:
      title: ''
      text: |
        <h2 class="experience-section-title">Recognition</h2>

        <ul class="experience-recognition-list">
          <li><strong>Secure Code Warrior Top Placement</strong><span>GM JEDI, 2024</span></li>
          <li><strong>Geek Week Debate Team Winner</strong><span>General Motors Geek Week, 2024</span></li>
          <li><strong>Geek Week Overall Annual Top Placement</strong><span>General Motors Geek Week, 2022 and 2024</span></li>
          <li><strong>Hackathon Team Winner</strong><span>General Motors Geek Week, 2022</span></li>
        </ul>
    design:
      css_class: "wide-block experience-recognition"
---
