# The Shape of the Game

An interactive editorial exhibit on football formations — built around the 12 tactical shapes used by teams at the 2026 FIFA World Cup's Round of 32.

**Live site:** https://crbikebike.github.io/shape-of-soccer/

## What it is

A single-page, single-file site styled as an editorial "matchday dossier" rather than a plain reference tool:

- **Filmstrip navigation** — 12 formations (4-3-3, 4-2-3-1, 3-5-2, 5-4-1, and more), each nav item rendering a live mini pitch-diagram thumbnail of that shape.
- **Team rosters** — every formation lists the Round of 32 teams that ran it, as flag-colored chips.
- **"See a goal"** — for the three most-picked formations, an animated sequence walks a ball through a typical build-up and finish, with a short attack/defend explainer alongside it.
- **Position exhibit labels** — click any player marker on the pitch to read about that position, with a Legend / Golden Era / Modern player example for each.

## Stack

No framework, no build step — one self-contained `index.html` (inline CSS + vanilla JS). Fonts (Fraunces, Source Serif 4, Barlow Condensed, JetBrains Mono) are pulled from Google Fonts; everything else, including the hero illustration, is embedded directly in the file.

## Running locally

Just open `index.html` in a browser, or serve the directory with any static file server:

```
python3 -m http.server 8000
```

## Deployment

Pushes to `main` auto-deploy to GitHub Pages via `.github/workflows/static.yml`.
