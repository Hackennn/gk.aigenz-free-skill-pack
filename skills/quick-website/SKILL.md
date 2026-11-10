---
name: quick-website
description: Build a clean, mobile-friendly one-page website (landing page, portfolio, link-in-bio, event page) from a short brief, as a single index.html with no build step. Use when the user asks for a simple website, landing page or portfolio page, or types "/quick-website".
---

# Quick website

## 1. Take the order (bubble-tea style)

Collect the brief, asking ONE question only for what is missing:
- **WHO** visits it, and **WHAT** they should do (buy, book, follow, contact)
- **CONTENT**: name, tagline, 3 key points, call to action, contact / links
- **STYLE**: 2–3 words (e.g. "soft pastel, cute", "dark, premium tech", "clean, minimal") plus brand colors if any

## 2. Build

- One `index.html` with inline CSS (and a little inline JS only if needed). No frameworks, no build tools.
- Sections in order: hero (headline + subline + button) → 3 benefits → proof (testimonials or numbers, only if the user gave real ones) → FAQ (optional) → final call to action → footer.
- Mobile first: readable at 375px wide, no sideways scrolling, buttons at least 44px tall.
- CSS variables for colors, good contrast, system fonts or one Google Font.
- Never invent testimonials, prices or stats. Use clearly marked placeholders like `[Your review here]`.

## 3. Check

- Open the page in a browser at phone width and desktop width. Fix overflow and contrast problems.
- Tell the user how to open it (double-click `index.html`) and how to publish it for free (e.g. GitHub Pages or Netlify Drop).
