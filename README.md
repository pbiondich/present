# Presentations

A static site hosting presentation decks by Jamie Thomas (Regenstrief Institute · Global Health Informatics).

## Structure

- `index.html` — landing page / chooser. Add a new `<a class="card">` block for each new deck.
- `moh-rg-kickoff-v2.html` — first deck: NDoH × Regenstrief six-month kickoff.
- `regenstrief-logo.png` — shared logo asset.

## Publishing on GitHub Pages

1. Create a new repo (e.g. `presentations`) and drop all files in `release/` at the repo root.
2. In repo **Settings → Pages**, set source to `main` / `/ (root)`.
3. Visit `https://<your-username>.github.io/presentations/`.

## Adding a new deck

Each deck is a single self-contained HTML file. To add one:

1. Place the new `your-deck.html` in the repo root.
2. Copy the `<a class="card">` block in `index.html`, update the `href`, title, label, pill date, and body copy.
3. Bump the `.count` in the section header.

## Notes

- Decks are built with React + Babel inlined — they work fully offline.
- Each deck remembers its last-viewed slide in `localStorage`.
- Use arrow keys or tap/click the edges to navigate. `P` prints to PDF.
