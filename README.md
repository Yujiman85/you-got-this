# You Got This 💪

A single-page site that shows a random affirmation every time you visit.

**Live site:** https://yujiman85.github.io/you-got-this/

## How it works

The site is a static `index.html` (HTML, CSS, and a small bit of JavaScript —
no build step, no dependencies). The affirmations live in a separate
`affirmations.json` file. On load (and whenever you tap **Give me another**), the
JavaScript fetches that list and picks a random affirmation.

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

Open `affirmations.json` and edit the `affirmations` array. Each entry is one
string. Commit and push — GitHub Pages redeploys automatically.

> Note: because the page loads `affirmations.json` over HTTP, opening
> `index.html` directly from disk (`file://`) won't fetch the list. View it
> through the live GitHub Pages URL, or a local server
> (`python3 -m http.server`), to see the affirmations.

## Hosting (GitHub Pages)

Served from the `main` branch root via GitHub Pages
(Settings → Pages → Source: Deploy from a branch → `main` / `/root`).

## Sources

The affirmations were drawn and adapted from reputable mental-health and
positive-psychology resources, chosen to be believable and empowering, and
phrased in the second person ("you") so they read as spoken to the reader —
present tense, not toxic positivity:

- Healthline — [Affirmations for Anxiety](https://www.healthline.com/health/mental-health/affirmations-for-anxiety), [Affirmations for Depression](https://www.healthline.com/health/mental-health/affirmations-for-depression)
- Mindful.org — [Benefits of Mindful Affirmations](https://www.mindful.org/5-benefits-of-including-mindful-affirmations-in-your-daily-routine/), [You Are Enough](https://www.mindful.org/build-resilience-by-staying-in-the-moment-2/)
- PositivePsychology.com — [Self-Love Exercises](https://positivepsychology.com/self-love-exercises-worksheets/), [Self-Compassion Techniques](https://positivepsychology.com/how-to-practice-self-compassion/), [Daily Affirmations: The Science](https://positivepsychology.com/daily-affirmations/)
- Psychology Today — [How to Use Self-Affirmations](https://www.psychologytoday.com/us/blog/click-here-for-happiness/202204/how-to-use-self-affirmations), [Affirmations for Difficult Family](https://www.psychologytoday.com/us/blog/between-the-generations/202412/how-to-use-affirmations-to-cope-with-difficult-family-members)
