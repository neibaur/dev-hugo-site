---
title: 'Education'
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
        <h2 class="education-section-title">Certifications</h2>

        {{< display_list key="certifications" type="all" header="" >}}
    design:
      css_class: "wide-block education-certifications"

  - block: education
    content:
      username: me
    design:
      date_format: 'January 2006'

  - block: markdown
    content:
      title: ''
      text: |
        <h2 class="education-section-title">Languages & Communication</h2>

        <div class="education-language-list">
          <div>
            <strong>English</strong>
            <span>Native</span>
          </div>
          <div>
            <strong>Mandarin Chinese</strong>
            <span>Fluent / professional working proficiency</span>
          </div>
          <div>
            <strong>Spanish</strong>
            <span>Basic</span>
          </div>
        </div>
    design:
      css_class: "wide-block education-languages"
---
