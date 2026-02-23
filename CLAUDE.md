# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

GitHub profile landing page for [@verygoodmurph](https://github.com/verygoodmurph). Single-page static site served via GitHub Pages from `index.html` at the repository root.

## Tech Stack

- Vanilla HTML/CSS/JavaScript — no frameworks, no build step
- Google Fonts (Cormorant + DM Sans)
- Static hosting via GitHub Pages

## Development

Open `index.html` directly in a browser. No install or build steps.

## Design Direction — Early PlayStation Soft Core

- **Aesthetic**: PS1 boot screen dreaminess — warm void, floating translucent geometry, bloom glow, film grain. Dark-first.
- **Palette**: Warm dark (`#1A1618`), dusty rose accent (`#C49A92`), warm off-white text (`#E0D6CC`). Light mode: parchment cream (`#F2ECE4`).
- **Typography**: Cormorant (italic serif display) + DM Sans (geometric sans body)
- **Background**: CSS-only floating geometric shapes (circle, triangle, diamond, cross) referencing PS button iconography. Radial bloom glows. SVG film grain overlay.
- **Theme**: Dark default. Light/dark toggle via `data-theme` on `<html>`, CSS variables, localStorage persistence, respects `prefers-color-scheme`
- **Motion**: Staggered `fadeUp` entrance, continuous `drift` float on background shapes, `prefers-reduced-motion` respected
