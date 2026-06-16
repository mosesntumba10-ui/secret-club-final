# SECRET CLUB® — Project README
**LA MESA NO ES PARA TODOS**

---

## Overview

SECRET CLUB® is a luxury streetwear brand website built with pure HTML, CSS, and vanilla JavaScript. The design language is built around exclusivity, ambition, and identity — dark aesthetics with a bold red accent palette.

---

## Project Structure

```
secretclub/
├── README.md                  ← You are here
│
├── pages/                     ← Standalone site pages
│   ├── index.html             ← Homepage
│   ├── collections.html       ← Collections page
│   ├── lookbook.html          ← Lookbook / editorial
│   └── about.html             ← About / The Club
│
├── variants/                  ← Color theme variants
│   ├── red-black.html         ← Red + Black (default)
│   ├── gold-black.html        ← Gold + Black (luxury)
│   └── white-minimal.html     ← White + Minimal (clean)
│
└── split/                     ← Modular split files
    ├── style.css              ← Shared stylesheet
    ├── main.js                ← Shared JavaScript
    └── template.html          ← Base HTML shell
```

---

## Design System

### Colors
| Token          | Value     | Usage                          |
|----------------|-----------|--------------------------------|
| `--black`      | `#050505` | Primary background             |
| `--black2`     | `#111111` | Secondary background           |
| `--dark`       | `#181818` | Card / surface background      |
| `--white`      | `#FFFFFF` | Primary text                   |
| `--silver`     | `#C0C0C0` | Secondary text / labels        |
| `--accent`     | `#CC0000` | Brand red — CTAs, highlights   |
| `--accent-dark`| `#8B0000` | Deep red — gradients, glows    |

### Typography
| Role    | Font        | Usage                        |
|---------|-------------|------------------------------|
| Display | Bebas Neue  | Headlines, logos, big titles |
| Body    | Inter       | Body copy, labels, nav       |

### Cursor
Custom crosshair cursor made of:
- A small red dot (center)
- Horizontal + vertical hairlines in red
- A lagging ring that follows with easing
- On hover: expands and flips to white

---

## Pages

### `index.html` — Homepage
Full landing experience with:
- Loader animation
- Hero section with parallax suit symbols
- Red ticker bar
- Collections preview grid
- Manifesto section
- Lookbook editorial grid
- Club philosophy
- Upcoming drop teaser
- Instagram hub
- Join CTA
- Contact section

### `collections.html` — Collections
- Full 6-card product grid
- Each card has number, title, description
- Hover reveals description with slide-up animation

### `lookbook.html` — Lookbook
- Full masonry-style editorial grid
- 8 visual panels across a 12-column grid
- Campaign labels and suit symbols on each cell

### `about.html` — About / The Club
- Brand stats (drops, pieces, members)
- Brand philosophy text
- Value cards: Exclusivity, Identity, Ambition, Community

---

## Color Variants

| File               | Accent Color | Mood          |
|--------------------|--------------|---------------|
| `red-black.html`   | `#CC0000`    | Bold, aggressive, default |
| `gold-black.html`  | `#B8860B`    | Luxury, premium, elite    |
| `white-minimal.html` | `#FFFFFF`  | Clean, editorial, minimal |

To create a new variant, change `--accent` and `--accent-dark` in `:root` and swap gradient hues in card visuals.

---

## Split Files

| File            | Purpose                                      |
|-----------------|----------------------------------------------|
| `style.css`     | All styles — import via `<link>` in any page |
| `main.js`       | Cursor, loader, GSAP reveals, scroll nav     |
| `template.html` | Minimal HTML shell with nav + footer wired   |

---

## Dependencies

All loaded via CDN — no build step required.

```html
<!-- Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">

<!-- GSAP + ScrollTrigger -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.5/gsap.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.5/ScrollTrigger.min.js"></script>
```

---

## Brand Guidelines

- **Tagline:** LA MESA NO ES PARA TODOS
- **Instagram:** [@secretclub.cl](https://www.instagram.com/secretclub.cl)
- **Suit symbols used:** ♠ ♦ ♣ (no ♥ — intentional)
- **Tone:** Exclusive, confident, minimal copy
- **Never use:** rounded corners, bright colors, casual fonts

---

## Quick Start

1. Open any `.html` file directly in a browser — no server needed
2. To use split files, ensure `style.css` and `main.js` are in the same folder as your HTML
3. To switch color themes, open a variant file from `/variants/`

---

*SECRET Club® © 2025 — Access must be earned.*
