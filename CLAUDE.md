# Project Context for Claude Code

## Who this project is for

Felix (GitHub: FelixUnger66) is a complete beginner learning to build professional-looking websites for businesses, using Claude Code as his primary build tool. This file gives any Claude Code session full context on this specific project without needing prior conversation history.

**Location/environment constraints (important, don't assume standard US setup):**
- Based in Vienna, Austria
- Uses an Austrian/German keyboard layout and German-language Windows interface
- The `@` symbol does not type reliably via keyboard shortcuts on his system (AltGr+Q and Ctrl+Alt+Q have both failed) — when he needs to enter an `@` in a terminal or config, the reliable workaround is typing it in Notepad first, then copy-pasting (right-click paste or Shift+Insert) rather than typing directly in the terminal
- Git Bash does not support standard Ctrl+V paste — use right-click or Shift+Insert instead

## Project goal

**Not** pursuing a traditional software developer career path (no plans for algorithm-heavy interview prep, CS fundamentals, job applications). The actual goal is:

> Build professional-looking, deployed websites for real businesses (clients), using Claude Code as the primary build tool.

This means the practical skill bar is: understand enough HTML/CSS to read, sanity-check, and manually tweak what Claude Code generates — not to hand-code everything from scratch, and not to pass technical interviews.

## About this project: "Grounded" coffee shop site

A single-page website for a fictional/practice neighborhood coffee shop called "Grounded", used both as a portfolio-style build and as the vehicle for learning real HTML/CSS concepts hands-on (as opposed to the separate, unrelated practice files in Felix's `my-website` repo, which this project has been split out from).

**Files:**
- `index.html` — the page structure (renamed from `grounded.html` on 2026-08-22 so Vercel's static hosting can find it as the default entry point at the site root — Vercel looks for `index.html` by default and was 404'ing without it)
- `grounded.css` — all styling

**Current structure/content of the page** (in order): a `.page-wrapper` div containing a centered nav bar (`.site-nav`, links to Home/Menu/Contact via anchor links), a header with the site name (`<h1>Grounded</h1>`), a welcome section with a hero image, intro paragraph, and a "View Full Menu" call-to-action button, a menu section listing items with prices (Espresso, Cappuccino, Warm Croissant) using flexbox rows (`.menu-item`), and a footer with address/phone/hours.

**Styling notes:**
- Color palette: warm coffee-shop tones — background `#F5EFE6` (cream), text `#3B2A20` (dark brown), accents/headers `#4B3223` (deep brown), menu item background `#EAD9C4` (tan)
- Fonts: Google Fonts `Fraunces` (serif, used for headings and the CTA button) and `Nunito` (sans-serif, body text) — loaded via `<link>` tags in the `<head>`
- Layout uses `max-width` + `margin: 0 auto` centering on `.page-wrapper`, and `display: flex` for the nav bar and menu item rows
- `.cta-button` has a hover effect (background color change, slight lift via `transform: translateY`, box-shadow)

**HTML/CSS concepts Felix has learned hands-on so far** (relevant to reading/tweaking this code): tags/elements, document structure (`<!DOCTYPE>`, `<html>`, `<head>`, `<body>`), headings/paragraphs/links/images, the `href`/`src`/`alt` attributes, CSS rule anatomy (selector/property/value), external stylesheets via `<link rel="stylesheet">`, the box model (content/padding/border/margin), classes (`.name` in CSS vs `class="name"` in HTML), `<div>` as a generic container, Flexbox (`display: flex` for row layouts), `max-width` + `margin: 0 auto` centering, and the structural difference between CSS (flat, order-independent rules) and HTML (nested hierarchy).

**Not yet covered, but expect it to come up naturally as this project grows**: lists (`<ul>`/`<li>`), forms (`<form>`, `<input>`, `<button>`), CSS Grid, media queries/responsive design mechanics, semantic tags (`<header>`, `<nav>`, `<footer>`, `<section>` — note: some of these are already used in the HTML even though the underlying concept of "semantic tags" hasn't been explicitly taught yet).

## Repository

This project lives at `C:\Users\FelixPC\Projects\grounded` and is pushed to its own GitHub repo: `FelixUnger66/grounded-coffee-shop` (public). It was split out from Felix's general `my-website` practice repo to keep this project separate from unrelated practice files (`test.html`, `style.css`), as it's evolving into a more polished, portfolio/client-style build.

## Working style / constraints for how to assist Felix

- Explain new technical terms in plain English the moment they appear — this was explicitly requested and re-requested; not optional
- Proceed step-by-step, one action at a time, confirm the result (ideally via him showing output/screenshot) before moving to the next step — do not batch multiple untested steps together
- Do not assume prior knowledge of anything outside what's documented in this file as already covered
- Felix is capable and engaged, but new to this entire domain — avoid making him feel behind for not knowing standard jargon; treat every "what does X mean" question as reasonable, not remedial
- Goal orientation: prioritize practical, client-facing website-building skill over CS-fundamentals depth or algorithmic interview prep
