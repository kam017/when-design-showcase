# When Design + Messaging System — Showcase

A two-page static showcase of the When design system.

- **Visual** (`/`) — Color palette, type scale, primitives (buttons, inputs, chips, tab strip, cards), motion samples.
- **Voice** (`/voice`) — Voice & tone guidelines, words to use and avoid, surface-by-surface copy patterns.

## Stack

Plain HTML + CSS + the system fonts. No build step, no framework, no dependencies.

## Develop locally

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy

Configured for Vercel as a static site (`vercel.json`). Push to Vercel and it'll serve `index.html` + `voice.html` directly.

## Files

- `index.html` — Visual page
- `voice.html` — Voice page
- `showcase.css` — Single stylesheet (brand tokens + chrome + primitive styles)
- `when-logo.svg` — The When wordmark
- `vercel.json` — Deploy configuration
