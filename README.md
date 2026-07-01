# Figura

A web app for mathematics teachers to create clean, labelled, exam-ready diagrams — shapes, graphs, charts, networks, trees, Venn diagrams, circles, 3D solids, bearings, number lines, tables, clocks/dice/spinners, algebra tiles and more — and export them as transparent PNG or SVG to drop straight into exams and worksheets.

## Running it

Figura is a single self-contained file, `index.html`. Just open it in a modern browser (Chrome or Edge recommended) — no install or build step.

Some features load libraries from a CDN and so need an internet connection:
- **MathJax / MathQuill** — the live maths editor and rendered maths labels.
- **Google Fonts (Lexend)** — the interface font.

## Hosting (make it available anywhere)

Because it's a static file, it can be hosted for free. See the deploy steps below (GitHub Pages).

## Notes

- Saved canvases live in each browser's local storage (per-machine). Cross-device sync would need a backend (a future phase).
- Export: "Download PNG" gives a high-res transparent PNG; "Export SVG" gives a vector file; "Copy image" copies straight to the clipboard for pasting into Word.

## Tech

Vanilla HTML/CSS/JavaScript, SVG rendering, no framework. MathJax (SVG output) for rendered maths, MathQuill for live maths input.
