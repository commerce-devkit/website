# Commerce DevKit website

This repository contains the source for the upcoming
[commerce-devkit.org](https://commerce-devkit.org) website. The site is built
with Hugo, uses the Ananke theme as a starter baseline, and is deployed to
GitHub Pages.

## Requirements

- Hugo Extended `0.160.0` or newer
- Git submodules

## Local development

1. Initialize the theme submodule:

   ```bash
   git submodule update --init --recursive
   ```

2. Start the local development server:

   ```bash
   hugo server
   ```

3. Open `http://localhost:1313/`.

## Production build

```bash
hugo --gc --minify
```

## Adding news posts

Create news posts with the dedicated archetype and a date-prefixed filename:

```bash
hugo new --kind news content/news/2026-05-30-my-update.md
```

Guidelines:

1. Use the `YYYY-MM-DD-slug.md` filename pattern so News stays chronologically scannable in the repository.
2. Keep the first paragraph or `summary` concise because it is reused in News listings and metadata.
3. Add `tags` when they will help future filtering or tag-cloud navigation.

Example front matter:

```yaml
---
title: "My update"
date: 2026-05-30T10:00:00+02:00
draft: false
summary: "One-sentence summary for listings and metadata."
tags:
  - release
  - website
---
```

## Deployment

Pushes to `main` deploy through GitHub Actions to GitHub Pages. The custom
domain is configured with `static/CNAME`.
