# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

The public website for **Kodeaben** — Anders Stensgaard's freelance software engineering consultancy. It serves as his primary online presence: showcasing services, past client work, and providing a direct contact point for potential clients.

The site is intentionally simple — a single scrolling HTML page, no build tooling, no framework. It will be served at `kodeaben.com` via GitHub Pages once the DNS is cut over from the current Squarespace site. To preview locally, open `index.html` directly in a browser.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The entire site — Nav, Hero, Services, Work, Contact, Footer |
| `style.css` | Site-specific layout and component styles |
| `CNAME` | GitHub Pages custom domain (`kodeaben.com`) |
| `design-system/` | Brand tokens, component patterns, logo |

## Design system

All tokens live in `design-system/colors_and_type.css` (CSS custom properties). `index.html` imports it directly — no build step, no npm.

- **Colors:** `var(--color-primary)` (lilac), `var(--color-secondary)` (sage), `var(--color-accent)` (tan), `var(--color-fg)` (charcoal), `var(--color-bg)` (cream)
- **Shadows:** Flat comic-book offset style — `var(--shadow-xs/sm/md/lg/xl)`
- **Borders:** `var(--border-thin/base/thick)` — thick charcoal outlines are a core motif
- **Icons:** Lucide CDN (`unpkg.com/lucide@latest`), initialized via `lucide.createIcons()`
- **Fonts:** Nunito (display/body) + JetBrains Mono — auto-loaded from Google Fonts inside `colors_and_type.css`
- Component HTML reference patterns: `design-system/preview/`

Never hardcode hex values in `style.css` — always use CSS variables.

## Sections (in order)

1. **Nav** — sticky floating pill navbar
2. **#hero** — headline + logo visual + two CTAs
3. **#services** — 5 service cards in a responsive grid
4. **#work** — 7 client project cards (SEGES, OK emobility, BankData, LEGO, Danske Bank ×2, Intelligent Systems)
5. **#contact** — mailto CTA, sage-tinted background
6. **Footer** — brand + copyright

## Deployment

Push to `main` → GitHub Pages serves the repo root. The `CNAME` file handles the custom domain. No build command needed.

## Brand voice

Warm, direct, slightly witty. Sentence case everywhere. Short sentences. The cartoon monkey mascot does the expressive heavy lifting — no emoji in copy.
