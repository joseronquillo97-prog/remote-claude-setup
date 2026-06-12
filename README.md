# Calculator

A simple, mobile-friendly calculator webapp.

**Live site:** https://joseronquillo97-prog.github.io/remote-claude-setup/
(auto-deploys from `main` via GitHub Pages)

## What it does

- Basic arithmetic: add, subtract, multiply, divide
- Extras: percent, sign toggle (±), decimal input, chained operations
- Full keyboard support: digits, `+ - * /`, `Enter` (=), `Esc` (clear), `Backspace`
- Pure static HTML/CSS/JS, no build step — works great on iPhone

## Local development

No tooling needed — just open `index.html` in a browser.

## Deployment

Deployed on **GitHub Pages** via GitHub Actions
(`.github/workflows/deploy-pages.yml`). Every push to `main` redeploys
the site automatically — no accounts or tokens needed beyond the repo
itself.
