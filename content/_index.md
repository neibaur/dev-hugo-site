---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '0rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      show_education: false
      show_ongoing: false
      link_interests: false
      # Show a call-to-action button under your biography? (optional)
      button:
        text:
        url:
      headings:
        about: 'Professional Summary'
        education: ''
        interests: ''
        ongoing: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: rounded # Options: circle (default), square, rounded

  - block: tech-stack
    content:
      title: Tech Stack
      categories:
        - name: Languages & Scripting
          items:
            - name: Python
            - name: SQL
        - name: Cloud & DevOps
          items:
            - name: Terraform
            - name: GitHub Actions
            - name: Docker
            - name: Kubernetes
            - name: Cloudflare
            - name: CI/CD
        - name: Data Platforms
          items:
            - name: Azure Databricks
            - name: PostgreSQL
            - name: Supabase
            - name: ETL Pipelines
        - name: Analytics & BI
          items:
            - name: Power BI
            - name: Looker Studio
            - name: Cognos
            - name: Tableau
        - name: Engineering Practices
          items:
            - name: REST APIs
            - name: Infrastructure as Code
            - name: DevSecOps
            - name: Agile
            - name: Automated Testing
    design:
      css_class: "wide-block"

  - block: markdown
    content:
      title: Featured Projects
      text: |
        <div class="landing-card-grid">
          <article class="landing-card">
            <div>
              <h3>Cloudflare Governance Platform</h3>
              <p>Terraform + Python + GitHub Actions platform for security audits, remediation workflows, policy validation, and infrastructure governance automation.</p>
            </div>
            <div class="landing-tags">
              <span>Terraform</span>
              <span>Python</span>
              <span>GitHub Actions</span>
              <span>Cloudflare</span>
              <span>IaC</span>
            </div>
          </article>

          <article class="landing-card">
            <div>
              <h3><a href="/projects/nhtsa-recall-intelligence/">NHTSA Data Platform</a></h3>
              <p>API ingestion and analytics platform using real-world vehicle safety data, medallion-style data modeling, Supabase/PostgreSQL, and Power BI dashboard integration.</p>
            </div>
            <div class="landing-tags">
              <span>Python</span>
              <span>APIs</span>
              <span>Supabase</span>
              <span>PostgreSQL</span>
              <span>Power BI</span>
            </div>
          </article>

          <article class="landing-card">
            <div>
              <h3><a href="https://100daydash.blog/">100DayDash Engineering Blog</a></h3>
              <p>Public engineering journal documenting platform engineering, DevSecOps, CI/CD, observability, automation, and dashboard development.</p>
            </div>
            <div class="landing-tags">
              <span>Technical Writing</span>
              <span>DevSecOps</span>
              <span>CI/CD</span>
              <span>Dashboards</span>
              <span>Automation</span>
            </div>
          </article>
        </div>
    design:
      css_class: "wide-block"

  - block: markdown
    content:
      title: Currently Building
      text: |
        - Cloudflare governance and remediation platform using Terraform, GitHub Actions, and Python
        - Public 100-day engineering initiative documenting cloud infrastructure and data platform development
        - NHTSA analytics platform using API ingestion, medallion-style architecture, Supabase, and Power BI
        - DevSecOps workflows with CodeQL, Dependabot, automated validation, and CI/CD governance
        - Dashboard engineering projects using Power BI, Looker Studio, Astro, Hugo, and Python visualization tools
    design:
      css_class: "wide-block"

  - block: markdown
    content:
      title: Latest Engineering Notes
      text: |
        <div class="landing-link-row">
          <a class="landing-link-card" href="https://100daydash.blog/">
            <strong>100DayDash Blog</strong>
            <span>Daily public notes on platform engineering, DevSecOps, automation, observability, and dashboard development.</span>
          </a>
          <a class="landing-link-card" href="/blog/">
            <strong>Portfolio Blog</strong>
            <span>Technical writing and project notes published on this site.</span>
          </a>
        </div>
    design:
      css_class: "wide-block"

  - block: markdown
    content:
      title: ''
      text: |
        {{< bio_grid >}}
          {{< display_list key="certifications" type="featured" header="Core Certifications" >}}
          {{< display_list key="awards" type="featured" header="Leadership & Recognition" >}}
        {{< /bio_grid >}}
    design:
      columns: 2
      css_class: "wide-block compact-recognition"
---
