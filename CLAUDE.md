# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Design Process assignment (DesignBuildShip course) — a showcase of the best characters from anime and animated comedy, presented through 20 distinct visual design variations. Built entirely with HTML and CSS. No JavaScript, no external images, no external fonts.

## Constraints

- **HTML and CSS only** — no JavaScript whatsoever
- No external CDN resources (fonts, images, libraries)
- All interactivity uses pure CSS (`:hover`, `:focus`, `:target`, `transition`, `@keyframes`)
- Attribute bar widths use inline `style="width: X%"` — this is intentional, not JS

## Architecture

```
Assignment1DesignProcess/
├── index.html              # Gallery landing page — links to all 20 variations
├── css/index.css           # Gallery page styles
├── v1-simpsons/            # Springfield Showcase — yellow/blue, donut-ring stats, bounce hover
├── v2-familyguy/           # Quahog Chronicles — comic panels, CSS card-flip, bar charts
├── v3-anime/               # Sakura Clash — asymmetric manga grid, cherry blossoms, neon gradients
├── v4-dc/                  # Gotham Files — dark panels, hex avatars, star ratings, grayscale hover
├── v5-marvel/              # Hero Spotlight — cinematic red/gold, featured hero, power bars
├── v6-matrix/              # The Construct — terminal green-on-black, digital rain, glitch
├── v7-reddit/              # r/AnimeAndCartoons — forum layout, vote arrows, stat pills
├── v8-vaporwave/           # Neon Dreams — pink/cyan/purple, sunset gradients, frosted glass
├── v9-swiss/               # Helvetica Protocol — B&W + red, typography-driven, ultra-minimal
├── v10-cyberpunk/          # Night City — neon yellow/cyan, angular clip-paths, HUD bars
├── v11-newspaper/          # The Daily Toon — cream paper, multi-column, drop caps, serif
├── v12-instagram/          # InstaGrid — social feed, story circles, hashtag stats
├── v13-gameboy/            # Select Your Fighter — arcade neon, HP bars, INSERT COIN
├── v14-spotify/            # Now Playing — dark theme, playlist rows, Now Playing bar
├── v15-ghibli/             # Spirited Gallery — soft pastels, watercolor blobs, dot ratings
├── v16-horror/             # The Crypt — blood red on black, pulsing vignette, flicker
├── v17-y2k/                # GeoCities Shrine — chaotic Y2K, marquee, rainbow, bevel borders
├── v18-bauhaus/            # Form Follows Function — Mondrian grid, primary colors, geometric
├── v19-noir/               # Case Files — sepia/parchment, file folders, venetian blinds
└── v20-steampunk/          # The Brass Registry — brass/copper, gears, porthole avatars
```

Each variation folder contains `index.html` + `style.css` and is self-contained. All 20 display the same 21 characters (3 per series from: Naruto, Jujutsu Kaisen, The Simpsons, Family Guy, South Park, Bob's Burgers, Rick and Morty).

## Navigation

- Gallery page links to each variation via themed cards
- Each variation has a "Back to Gallery" link
- V1–V7 have prev/next links to adjacent variations

## Character Data

Anime characters share attributes: Strength, Speed, Intelligence, Energy, Durability (1-10).
Comedy characters share attributes: Humor, Chaos, Intelligence, Heart, Resilience (1-10).
Each character has a 2-sentence bio. Data is hardcoded identically in all 20 variation HTML files.
