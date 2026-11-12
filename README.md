# Sudoku Atlas

A responsive, browser-based guide to the 107 Sudoku techniques from the referenced conversation. It is a static site: no account, build step, or server is required.

## Open the site

Open `index.html` in a modern browser. For a local web address instead, open a terminal in this folder and run:

```sh
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## What’s included

- Six difficulty sections and a dedicated hash-routed page for each technique.
- Search, difficulty filters, previous/next lesson links, glossary, and browser-local learning progress.
- Two worked cases on every lesson page. Every case now displays a 9×9 Sudoku grid, and revealing each step highlights the cells involved. The first ten lessons have playable grids; every example shows candidate notes throughout the 9×9 grid. Black digits are starting clues, blue digits are placements, and technique-specific colors identify the pattern area. The advanced lessons use illustrative candidate grids; their contextual clue digits are not claimed as original clues from a sourced puzzle.
- The Easy → Full House lesson includes two interactive grids: one row and one column, each with eight filled cells and one missing digit.

Use the number buttons or keyboard digits to enter a grid answer. The example tabs, reveal controls, and progress button work entirely in the browser. Progress is saved in local storage on that device.

## Files

- `index.html` — page shell and asset references.
- `styles.css` — responsive layout and visual styling.
- `app.js` — navigation, search, interactive exercises, and progress.
- `content.js` — the six categories and 107 lesson entries.
- `grids.js` — interactive Sudoku boards for the first ten lessons.

The advanced examples are teaching diagrams and conditional deductions, not a verified collection of complete advanced Sudoku puzzles. Where a proof depends on an assumed pattern or uniqueness, the lesson says so.
