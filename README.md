# When Design + Messaging System — Showcase

A static showcase of the When design and messaging system: brand, visual identity, voice, and governance.

**Live:** https://when-design-showcase.vercel.app

## Pages

| Page | URL | Contents |
| --- | --- | --- |
| Design System | [`/`](https://when-design-showcase.vercel.app/) | Index / overview |
| Brand | [`/brand`](https://when-design-showcase.vercel.app/brand) | Story, audiences, messaging, naming, boilerplate |
| Visual Identity | [`/visual`](https://when-design-showcase.vercel.app/visual) | Logos, color palette, type scale, downloads |
| Voice & Tone | [`/voice`](https://when-design-showcase.vercel.app/voice) | Voice principles, words to use and avoid, copy patterns |
| Voice · Sales | [`/voice-sales`](https://when-design-showcase.vercel.app/voice-sales) | Sales-surface messaging and copy |
| Design | [`/design`](https://when-design-showcase.vercel.app/design) | Primitives, tokens, components |
| About / Governance | [`/governance`](https://when-design-showcase.vercel.app/governance) | Ownership, contribution, RFC process |

## Stack

Plain HTML + CSS with Google-hosted fonts (Merriweather, Material Symbols). No build step, no framework, no dependencies.

## Develop locally

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

Note: clean URLs (`/brand` instead of `/brand.html`) are a Vercel feature. Served locally, use the `.html` extension.

## Deploy

Static site on Vercel (`vercel.json` — `cleanUrls`, security headers, long-cache for fonts/SVG). The GitHub repo is connected to the Vercel project, so pushes to `main` deploy automatically. Internal working material (`_inbox/`, `STATUS_SWOT.md`) is excluded from the repo and the deploy via `.gitignore` / `.vercelignore`.

## Files

- `index.html`, `brand.html`, `visual.html`, `voice.html`, `voice-sales.html`, `design.html`, `governance.html` — the pages
- `showcase.css` — single stylesheet (brand tokens + chrome + primitive styles)
- `when-logo.svg`, `assets/` — wordmark and downloadable brand assets (logos, color tokens)
- `vercel.json` — deploy configuration
