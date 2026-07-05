# Agent Guidelines

Personal website of Josep Puig Ruiz. Jekyll site based on the [al-folio](https://github.com/alshedivat/al-folio) theme, deployed to GitHub Pages by `.github/workflows/deploy.yml` on push to `main`.

## Local development

```bash
docker compose up          # dev server at http://localhost:8080
docker compose up --build  # rebuild after dependency/Dockerfile changes
docker compose down        # stop and free port 8080
```

## Pre-commit checklist

1. Format: `npx prettier . --write` (first time: `npm install --save-dev prettier @shopify/prettier-plugin-liquid`)
2. Build locally with Docker and verify pages, images, and dark mode at http://localhost:8080

## Where things live

- `_pages/about.md` — home page content
- `_posts/` — blog posts (`YYYY-MM-DD-title.md`)
- `_news/` — announcements shown on the home page
- `assets/json/resume.json` — resume (JSON Resume format), rendered at `/resume/` by `_layouts/cv.liquid`
- `_data/socials.yml` — contact/social links
- `_config.yml` — site configuration

## Gotchas

- `_config.yml`: `url: https://puigruizjosep1.github.io` with empty `baseurl` (personal site). Quote YAML strings containing special characters.
- Upstream theme docs (CUSTOMIZE.md, FAQ.md, etc.) were removed from this repo; consult https://github.com/alshedivat/al-folio when needed.
