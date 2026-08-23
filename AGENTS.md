# Repository Guidelines

This repository contains Xianglin Yao's personal academic website, based on the
al-folio Jekyll theme.

## Before editing

- Preserve personal content in `_pages/`, `_news/`, `_projects/`,
  `_bibliography/`, `_data/`, and `assets/pdf/`.
- Keep Markdown front matter and YAML indentation valid.
- Keep `url` and `baseurl` consistent when changing deployment settings.
- Do not edit generated files in `_site/` or the `gh-pages` branch.

## Local checks

```bash
npx prettier . --write
docker compose up --build
```

The local site is served at <http://localhost:8080>. Verify navigation, images,
links, and dark mode before committing. Use `docker compose down` when finished.

For this personal GitHub Pages site, keep `url: https://YYYYXL1004.github.io` and
an empty `baseurl` in `_config.yml`.
