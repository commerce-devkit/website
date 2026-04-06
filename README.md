# Commerce DevKit website

This repository contains the source for the upcoming
[commerce-devkit.org](https://commerce-devkit.org) website. The site is built
with Hugo, uses the Ananke theme as a starter baseline, and is deployed to
GitHub Pages.

## Requirements

- Hugo Extended `0.148.2` or newer
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

## Deployment

Pushes to `main` deploy through GitHub Actions to GitHub Pages. The custom
domain is configured with `static/CNAME`.
