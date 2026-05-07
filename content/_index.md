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
      link_interests: true
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
          <a class="landing-card" href="/projects/cloudflare-governance-platform/">
            <div>
              <h3>Cloudflare Governance Platform</h3>
              <p>Infrastructure governance platform for automated security auditing, remediation workflows, and policy enforcement.</p>
            </div>
            <div class="landing-tags">
              <span>Terraform</span>
              <span>Python</span>
              <span>Policy Automation</span>
            </div>
          </a>

          <a class="landing-card" href="/projects/nhtsa-recall-intelligence/">
            <div>
              <h3>NHTSA Data Platform</h3>
              <p>Vehicle safety analytics platform for API ingestion, medallion-style modeling, relational storage, and dashboard-ready insights.</p>
            </div>
            <div class="landing-tags">
              <span>APIs</span>
              <span>Data Modeling</span>
              <span>Analytics</span>
            </div>
          </a>

          <a class="landing-card" href="/projects/100daydash-engineering-blog/">
            <div>
              <h3>100DayDash Engineering Blog</h3>
              <p>Public engineering journal documenting automation, platform delivery, observability, and dashboard development.</p>
            </div>
            <div class="landing-tags">
              <span>Technical Writing</span>
              <span>Observability</span>
              <span>Automation</span>
            </div>
          </a>
        </div>
    design:
      css_class: "wide-block landing-wide landing-featured"

  - block: markdown
    content:
      title: Engineering Notes
      text: |
        <div class="landing-link-row landing-link-row-single">
          <a class="landing-link-card" href="https://100daydash.blog/">
            <strong>100DayDash Blog</strong>
            <span>Public engineering journal documenting platform delivery, CI/CD governance, observability, automation, and dashboard development.</span>
          </a>
        </div>
    design:
      css_class: "wide-block landing-wide landing-notes"
---
