# Yıldırım Family Heritage Website

## Overview
Trilingual (EN/DE/TR) static family heritage website for the Yıldırım family, emphasizing Ardahan roots and Trabzon connection.

## Tech Stack
- Single `index.html` with embedded CSS & JS — no build tools, no server
- **GSAP 3 + ScrollTrigger** (CDN) — scroll-driven animations, horizontal scroll sections, reveals
- **Lenis** (CDN) — buttery smooth scrolling
- **Canvas API** — custom gold particle system with mouse interaction
- Fonts: Cinzel Decorative (display), Cinzel (headings), Cormorant Garamond (body), Spectral (accent/italic)
- Theme: Deep midnight (#060610), gold accents (#c9a84c), luxury heraldic feel

## Structure
- `index.html` — Full website (all sections, styles, scripts, CDN imports)
- `favicon.svg` — Shield + sun SVG favicon
- `yildirim-family.png` — Coat of arms image

## Key Features
- **Preloader** — SVG shield path-draw animation + letter-by-letter "YILDIRIM" reveal
- **Custom cursor** — Gold dot + ring, hover state expansion (disabled on mobile)
- **Gold particles** — Canvas-based floating particles that react to mouse movement
- **Coat of arms parallax** — 3D tilt following mouse position via GSAP
- **Horizontal scroll** — Timeline and Gallery sections pinned with GSAP ScrollTrigger
- **3D tilt cards** — Origin cards (Ardahan/Trabzon) with mouse-tracking perspective + spotlight
- **Section reveals** — Staggered GSAP animations triggered on scroll

## i18n System
- JS translation object `T` with keys for `en`, `de`, `tr`
- `data-i18n` attributes on text elements, `data-i18n-placeholder` on inputs
- Language stored in `localStorage('yildirim-lang')`
- To add a translation key: add to all 3 language objects in `T`, then add `data-i18n="key"` to the HTML element

## Sections
1. Hero — Particle canvas + parallax coat of arms + character-by-character title animation
2. History — Ardahan & Trabzon origin story, 3D tilt origin cards, horizontal scroll timeline
3. Family — Empty section awaiting real data
4. Gallery — Horizontal scroll gallery with lightbox
5. Contact — Animated form fields + social links
6. Footer — Motto + copyright
