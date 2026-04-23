# Presentations

A static site hosting presentation decks by Paul Biondich, MD (Regenstrief Institute · Global Health Informatics · Founder, OpenMRS).

## Structure

- `index.html` — landing page / chooser. Add a new `<a class="card">` block for each new deck.
- `moh-rg-kickoff-v2.html` — NDoH × Regenstrief six-month kickoff (14 slides).
- `animation-playground.html` — Paul's Animation Playground, 16 studies in motion with varied transitions between slides.
- `regenstrief-logo.png` — shared logo asset.

## Publishing on GitHub Pages

1. Create a new repo (e.g. `presentations`) and drop all files in `release/` at the repo root.
2. In repo **Settings → Pages**, set source to `main` / `/ (root)`.
3. Visit `https://<your-username>.github.io/presentations/`.

## Adding a new deck

Each deck is a single self-contained HTML file. To add one:

1. Place the new `your-deck.html` in the repo root.
2. Copy an `<a class="card">` block in `index.html`, update the `href`, title, label, pill date, and body copy.
3. Bump the `.count` in the section header.

## Notes

- Decks are built with React + Babel inlined — they work fully offline.
- Each deck remembers its last-viewed slide in `localStorage`.
- Use arrow keys or tap/click the edges to navigate.
- The Animation Playground plays a different transition effect (push / dip / zoom / wipe / shutter / iris / overshoot) on every slide change.
- To save as PDF: use the browser's **Print** command (`Cmd/Ctrl + P`) and "Save as PDF" — each slide renders as its own page at the authored 1920×1080 size, no extra setup needed.
