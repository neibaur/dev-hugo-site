# AGENTS.md

Guidance for AI coding agents working in this repository.

## Repository Purpose

This is the source repository for [isaacneibaur.com](https://isaacneibaur.com), Isaac Neibaur's Hugo Blox portfolio. It is a static Hugo portfolio site, not a Python dashboard, Astro app, or monorepo. Keep changes lightweight and appropriate for a personal portfolio.

Production is generated from this repo and deployed by GitHub Actions to [`neibaur/github.io`](https://github.com/neibaur/github.io), which serves `isaacneibaur.com`.

## Branch Policy

- `main` is the production trunk branch. Treat it as always deployable.
- `dev` is only for experiments and should not be assumed to represent production.
- Prefer trunk-based development with small, atomic commits.
- Keep unrelated content, layout, dependency, and workflow changes in separate commits.

## What To Edit

- Authored content lives in `content/` and `data/authors/me.yaml`.
- Site configuration lives in `config/_default/`.
- Local Hugo Blox overrides live in `layouts/`.
- Local styles and media live in `assets/`.
- Public static downloads live in `static/uploads/`.

Do not edit generated output or vendored dependencies:

- `public/`
- `resources/`
- `.hugo_build.lock`
- `hugo_stats.json`
- `node_modules/`
- `_vendor/` unless explicitly updating Hugo Blox modules

## Hugo Blox Notes

This site uses Hugo Blox plus local custom shortcodes and partials. Do not replace or remove custom shortcodes such as:

- `display_list`
- `bio_grid`
- `landing_anchor`
- `sidebar_button`
- `sidebar_title`

These shortcodes are intentional portfolio building blocks. Preserve them when rewriting copy or moving content.

## Local Validation

For preview:

```bash
hugo server --disableFastRender
```

For a production-style build:

```bash
hugo --gc --minify
```

On Windows, if Hugo cannot access the default user cache, use a repo-local absolute cache path:

```powershell
hugo --gc --minify --cacheDir "$PWD\.hugo-cache"
```

Do not add Python, Astro, database, service-worker, or dashboard-style tooling unless the user explicitly asks for it. Prefer Hugo-native or small Node-based tooling only when it directly improves this static portfolio.

## Content Standards

- Keep portfolio content factual, current, and specific to Isaac's work.
- Remove or quarantine Hugo Blox starter/demo content that dilutes the personal brand.
- Use `_drafts/` for archived starter material that should not build into the public site.
- Keep public pages focused on biography, experience, education/certifications, projects, publications, events, and contact paths.
- Do not publish placeholder projects, template posts, sample talks, or sample slides.

## Deployment Context

Production deploys are cross-repo:

1. This repo is built by GitHub Actions.
2. Generated output from `public/` is pushed to `neibaur/github.io`.
3. `neibaur/github.io` serves `isaacneibaur.com`.

Any deployment or workflow change must account for that cross-repo publishing model.
