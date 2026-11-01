# Agent Instructions

## Communication
- The user writes in **Arabic**. Always reply in **English**.
- Keep replies **short, clear, simple, well-formatted** (Markdown, headers/bullets where useful).
- No filler, no long preambles. Explain only what is needed.

## Project
- Static single-file portfolio site. `index.html` contains everything: CSS (`<style>`), markup, and JS (`<script>`).
- Editable content lives in JS arrays between marker comments:
  `ACHIEVEMENTS`, `FOLLOWERS`, `BRANDS`, `SHOWCASE`, `SAHL`, `ALL_WORK`.
- The in-page **Studio** (secret 🚪 in the footer, password in `index.html`) edits those arrays and exports a new `index.html`.
- Images: `img/`, `All Work/`, `SAHL/`.
- Deploy: GitHub Pages via `CNAME` -> `ccp.ifeps.net`, repo `ramyhq/ccp`.

## Conventions
- Vanilla JS only, no build step, no dependencies.
- Escape user content with `esc()` / `escAttr()` before injecting HTML.
- Keep the `/* === X_START === */` / `/* === X_END === */` markers intact — export depends on them.
