# You Got This 💪

A single-page site that shows a random affirmation every time you visit.

**Live site:** https://yujiman85.github.io/you-got-this/

## How it works

The entire site is one static `index.html` file — HTML, CSS, and a small bit of
JavaScript with no build step and no dependencies. On load (and whenever you tap
**Give me another**), the JavaScript picks a random affirmation from the list in
`index.html`.

Features:
- **Random on every visit** — refresh for a new one.
- **"Give me another" button** — a fresh affirmation without reloading.
- **No-repeat logic** — never shows the same affirmation twice in a row (it
  remembers the last one via `localStorage`, so a reload won't repeat either).
- **Accessible** — semantic HTML, a live region so screen readers announce new
  affirmations, strong color contrast, a visible keyboard focus indicator, and
  respect for `prefers-reduced-motion`.
- **Responsive** — readable on phones and desktops.

## Editing the affirmations

Open `index.html` and edit the `affirmations` array near the bottom. Each entry
is one string. Commit and push — GitHub Pages redeploys automatically.

## Hosting (GitHub Pages)

Served from the `main` branch root via GitHub Pages
(Settings → Pages → Source: Deploy from a branch → `main` / `/root`).
