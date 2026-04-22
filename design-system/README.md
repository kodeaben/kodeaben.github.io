# Kodeaben Design System

## Overview
Kodeaben is a playful, personality-driven brand — anchored by a cartoon monkey mascot with thick outlines, soft rounded forms, and a muted-but-warm color palette. The brand sits at the intersection of **friendly tech** and **creative craft**: approachable and a little cheeky, but never unprofessional.

**Source:** Logo provided as `uploads/logo4.png` (copied to `assets/logo.png`)

---

## CONTENT FUNDAMENTALS

- **Tone:** Warm, direct, slightly witty. Never stiff or corporate.
- **Voice:** First-person "we" for the brand; second-person "you" for the user.
- **Casing:** Sentence case everywhere — not Title Case for body or CTAs.
- **Emoji:** Rare and intentional — the mascot/logo does the expressive heavy lifting.
- **Copy vibe:** Short sentences. No fluff. A little self-aware humor is fine.

---

## VISUAL FOUNDATIONS

### Colors
- **Lilac** `#D4B4D8` — primary brand background, from logo circle
- **Sage** `#6B8F80` — secondary, from monkey ears
- **Tan** `#C9B87A` — warm accent, from monkey face
- **Charcoal** `#2A2826` — outlines, text, thick borders
- **Cream** `#F6F2EA` — warm white surface/background
- **Deep Lilac** `#9B6EA8` — darker lilac for interactive states

### Typography
- **Display:** "Nunito" (rounded, friendly, Google Fonts) — matches the rounded cartoon aesthetic
- **Body:** "Nunito" regular — consistent family, easy reading
- **Mono:** "JetBrains Mono" — for code snippets

### Backgrounds
- Solid muted colors (cream, lilac tints); no complex gradients
- Subtle hand-crafted feel — sometimes a slight paper texture

### Borders & Outlines
- **Thick outlines** (2–3px solid charcoal) are a core design motif — inspired by the cartoon monkey's bold lines
- Border radius: generous — 12px for cards, 24–999px for pills/buttons, 50% for circles

### Shadows
- Offset shadows (4px 4px 0px charcoal) — flat/comic-book style, not blurred drop shadows
- Hover: shift to 2px 2px or 0px 0px to simulate "press"

### Corner Radii
- XS: 4px | SM: 8px | MD: 12px | LG: 20px | XL: 32px | Pill: 999px | Circle: 50%

### Animation
- Slight bounce on hover (transform: scale(1.03))
- Transitions: 150ms ease-out
- No heavy motion; subtle and snappy

### Iconography
- See ICONOGRAPHY section below
- Lucide icons (stroke-based, clean) preferred
- Icon stroke width: 2px to match charcoal outline motif

### Cards
- White or cream background
- 2px solid charcoal border
- 12–20px border radius
- 4px 4px 0 charcoal offset shadow
- Hover: shadow shrinks, card shifts slightly

---

## ICONOGRAPHY
- **Style:** Stroke-based line icons (Lucide CDN)
- **Stroke:** 2px, charcoal `#2A2826`
- **No filled icons** — the brand uses outlines (mirrors the logo)
- **Sizes:** 16px (inline), 20px (default), 24px (prominent)
- **CDN:** https://unpkg.com/lucide@latest/dist/umd/lucide.min.js

---

## FILE INDEX

| File | Contents |
|------|----------|
| `README.md` | This file — brand overview |
| `colors_and_type.css` | CSS variables for colors, type, spacing, radii, shadows |
| `assets/logo.png` | Primary logo (monkey mascot on lilac circle) |
| `preview/` | Design system card previews |
| `SKILL.md` | Agent skill definition |
