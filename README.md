# Remote Claude Setup

A mobile-friendly checklist webapp showing everything you need to enable to
control a local Claude Code session from your iPhone (Remote Control).

**Live site:** deployed on Vercel (auto-deploys from `main`).

## What it does

- Interactive checklist of every Remote Control requirement and setup step
- Progress bar with completion banner
- Progress saved in your browser (localStorage) — works great on iPhone
- Pure static HTML/CSS/JS, no build step

## Build steps (tracked in this repo's commit history)

1. **Scaffold the static app** — `index.html` with the checklist UI
2. **Initialize git + GitHub repo** — version control from the start
3. **Connect to Vercel** — import the repo at vercel.com/new; every push to
   `main` auto-deploys
4. **Iterate from anywhere** — edit via GitHub mobile app or Remote Control,
   push, and Vercel redeploys automatically

## Local development

No tooling needed — just open `index.html` in a browser.

## Deployment

Deployed on [Vercel](https://vercel.com) via GitHub integration:

1. Go to [vercel.com/new](https://vercel.com/new)
2. Import this repository
3. Framework preset: **Other** (static site, no build command)
4. Deploy — done. Every future `git push` redeploys automatically.

## Reference

- [Claude Code Remote Control docs](https://code.claude.com/docs/en/remote-control)
