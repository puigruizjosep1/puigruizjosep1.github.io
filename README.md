# puigruizjosep1.github.io

Personal website of Josep Puig Ruiz, built with [Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio) theme. Deployed to GitHub Pages via GitHub Actions on every push to `main`.

## Local development

```bash
docker compose up
# site at http://localhost:8080
```

## Structure

- `_pages/about.md` — home page
- `_posts/` — blog posts
- `_news/` — news/announcement items shown on the home page
- `assets/json/resume.json` — resume data ([JSON Resume](https://jsonresume.org/) format), rendered at `/resume/`
- `_config.yml` — site configuration

## Formatting

```bash
npx prettier . --write
```
