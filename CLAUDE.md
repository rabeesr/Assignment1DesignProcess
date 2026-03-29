# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Design Process assignment (DesignBuildShip course) — a showcase of the best characters from anime and animated comedy, presented through 7 distinct visual design variations. Built entirely with HTML and CSS. No JavaScript, no external images, no external fonts.

## Constraints

- **HTML and CSS only** — no JavaScript whatsoever
- No external CDN resources (fonts, images, libraries)
- All interactivity uses pure CSS (`:hover`, `:focus`, `:target`, `transition`, `@keyframes`)
- Attribute bar widths use inline `style="width: X%"` — this is intentional, not JS

## Architecture

```
Assignment1DesignProcess/
├── index.html              # Gallery landing page — links to all 7 variations
├── css/index.css           # Gallery page styles
├── v1-simpsons/            # Springfield Showcase — yellow/blue, donut-ring stats, bounce hover
│   ├── index.html
│   └── style.css
├── v2-familyguy/           # Quahog Chronicles — comic panels, CSS card-flip on hover, bar charts
│   ├── index.html
│   └── style.css
├── v3-anime/               # Sakura Clash — asymmetric manga grid, cherry blossoms, neon gradients
│   ├── index.html
│   └── style.css
├── v4-dc/                  # Gotham Files — dark panels, hexagonal avatars, star ratings, grayscale hover
│   ├── index.html
│   └── style.css
├── v5-marvel/              # Hero Spotlight — cinematic red/gold, featured hero, segmented power bars
│   ├── index.html
│   └── style.css
├── v6-matrix/              # The Construct — terminal green-on-black, digital rain, glitch, scanlines
│   ├── index.html
│   └── style.css
└── v7-reddit/              # r/AnimeAndCartoons — forum layout, vote arrows, stat pills, sticky sidebar
    ├── index.html
    └── style.css
```

Each variation is self-contained (own HTML + CSS) and displays the same 21 characters (3 per series from: Naruto, Jujutsu Kaisen, The Simpsons, Family Guy, South Park, Bob's Burgers, Rick and Morty).

## Navigation

- Gallery page links to each variation via cards
- Each variation has a "Back to Gallery" link and prev/next links to adjacent variations
- V1 ↔ V2 ↔ V3 ↔ V4 ↔ V5 ↔ V6 ↔ V7

## Character Data

Anime characters share attributes: Strength, Speed, Intelligence, Energy, Durability (1-10).
Comedy characters share attributes: Humor, Chaos, Intelligence, Heart, Resilience (1-10).
Each character has a 2-sentence bio. Data is hardcoded identically in all 7 variation HTML files.
