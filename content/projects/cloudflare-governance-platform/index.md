---
title: Cloudflare Governance & Remediation Platform
date: 2026-05-05
summary: Terraform, Python, and GitHub Actions system for Cloudflare security audits, policy validation, and optional drift remediation.
tags:
  - Python
  - Terraform
  - GitHub Actions
  - Cloudflare API
  - DevSecOps
---

Cloud automation project for auditing Cloudflare domain security posture and managing repeatable governance workflows through code.

<!--more-->

The system combines Python, Terraform, GitHub Actions, and the Cloudflare API to check configuration state, validate policy expectations, and optionally remediate drift. The work emphasizes Infrastructure as Code, scheduled audits, secure secret handling, automated validation, and repository governance patterns that support reliable cloud operations.

<div class="project-action-row">
  <a class="project-action" href="https://github.com/neibaur/cloudflare_IaC" target="_blank" rel="noopener">View GitHub Repository</a>
</div>

<div class="project-tech-list">
  <span>Python</span>
  <span>Terraform</span>
  <span>GitHub Actions</span>
  <span>Cloudflare API</span>
  <span>Infrastructure as Code</span>
  <span>DevSecOps</span>
  <span>Secret Management</span>
  <span>Scheduled Audits</span>
</div>

Current focus areas:

- Cloudflare security posture audits using Python and the Cloudflare API
- Terraform workflows for repeatable Infrastructure as Code validation
- GitHub Actions pipelines for scheduled audits and CI checks
- Secure secret handling for automation workflows
- Optional remediation workflows for configuration drift correction
- DevSecOps practices including Dependabot, CodeQL, branch protection, linting, and test checks

Design notes:

- Audit workflows run automatically, while remediation remains intentionally gated.
- Terraform and Python separate declarative infrastructure validation from API-driven audit logic.
- Secrets and real configuration inputs stay out of mock validation paths.
- CodeQL, Dependabot, Gitleaks, and branch protection support repository governance and operational reliability.
