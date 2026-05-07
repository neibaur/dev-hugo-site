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
      show_proof_points: true
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

  - block: markdown
    content:
      title: Featured Projects
      text: |
        <div class="landing-card-grid">
          <article class="landing-card">
            <div>
              <h3>Cloudflare Governance Platform</h3>
              <p>Governance automation platform for security audits, remediation workflows, policy validation, and infrastructure control.</p>
            </div>
            <div class="landing-tags">
              <span>Terraform</span>
              <span>Python</span>
              <span>Policy Automation</span>
            </div>
          </article>

          <article class="landing-card">
            <div>
              <h3><a href="/projects/nhtsa-recall-intelligence/">NHTSA Data Platform</a></h3>
              <p>Vehicle safety data platform for API ingestion, medallion-style modeling, relational storage, and dashboard-ready analytics.</p>
            </div>
            <div class="landing-tags">
              <span>APIs</span>
              <span>Data Modeling</span>
              <span>Analytics</span>
            </div>
          </article>

          <article class="landing-card">
            <div>
              <h3><a href="https://100daydash.blog/">100DayDash Engineering Blog</a></h3>
              <p>Public engineering journal documenting automation, platform work, observability, and dashboard development.</p>
            </div>
            <div class="landing-tags">
              <span>Technical Writing</span>
              <span>Observability</span>
              <span>Automation</span>
            </div>
          </article>
        </div>
    design:
      css_class: "wide-block landing-wide landing-featured"

  - block: markdown
    content:
      title: Latest Engineering Notes
      text: |
        <div class="landing-link-row">
          <a class="landing-link-card" href="https://100daydash.blog/">
            <strong>100DayDash Blog</strong>
            <span>Public notes on engineering projects, delivery tradeoffs, observability, and dashboard development.</span>
          </a>
          <a class="landing-link-card" href="/blog/">
            <strong>Portfolio Engineering Notes</strong>
            <span>Technical writing and project notes published on this site.</span>
          </a>
        </div>
    design:
      css_class: "wide-block landing-wide landing-notes"
---
