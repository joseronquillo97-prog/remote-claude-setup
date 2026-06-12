# Graphing Calculator

A mobile-friendly graphing calculator webapp with preset formulas that draw
shapes like a heart and a happy face.

**Live site:** https://raw.githack.com/joseronquillo97-prog/remote-claude-setup/main/index.html

## What it does

- Plots `y = f(x)` functions and implicit equations like `x^2 + y^2 = 9`
- **Text graphing with real formulas** — type any text and each letter
  outline is fitted with a Fourier series; the resulting parametric
  formulas (`x = ...; y = ...` with t in [0, 2π]) appear as editable
  equations in the list, the graph is drawn from those formulas, and a
  button copies them all
- Parametric equations: `x = cos(t); y = sin(t)`
- Preset shape examples: ❤️ Heart, 🙂 Happy face, 🌸 Flower, ∞ Infinity,
  〰️ Waves — each loads its formulas into the equation list so you can
  see and edit them
- Multiple equations at once, each in its own color
- Pan by dragging, pinch or scroll to zoom, zoom/reset buttons
- Formula syntax: `+ - * / ^`, implicit multiplication (`2x`, `4(x+1)`),
  functions `sin cos tan asin acos atan sqrt abs ln log exp`, constants
  `pi` and `e`
- Pure static HTML/CSS/JS, no build step — works great on iPhone

## Shape formulas

| Shape | Equation |
|---|---|
| Heart | `(x^2 + y^2 - 1)^3 = x^2 * y^3` |
| Flower (4-petal rose) | `(x^2 + y^2)^3 = 4(x^2 - y^2)^2` |
| Infinity (lemniscate) | `(x^2 + y^2)^2 = 4(x^2 - y^2)` |
| Happy face | circle + two small circles + a parabola smile with a domain trick: `y = 0.35x^2 - 2.3 + 0*sqrt(1.7 - abs(x))` |

## Local development

No tooling needed — just open `index.html` in a browser.

## Deployment

Served from `main` by the [raw.githack.com](https://raw.githack.com) CDN —
every push to `main` updates the live site after a short cache delay.

A GitHub Pages workflow (`.github/workflows/deploy-pages.yml`) also publishes
to the `gh-pages` branch on every push to `main`; enabling Pages in the repo
settings (Settings → Pages → deploy from `gh-pages`) makes the site available
at https://joseronquillo97-prog.github.io/remote-claude-setup/ as well.
