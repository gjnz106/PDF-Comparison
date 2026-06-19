# PDF Compare — DQT

A single-file, browser-based tool to **compare two revisions of a PDF** and **mark up** drawings — no install, no server, everything runs locally in the browser.

> Author: Dang Quoc Truong (DQT)

## Features

### Compare modes
- **Overlay** — blend Old/New revisions with an opacity slider.
- **Pixel Diff** — colored difference map (red = removed, green = added, grey = unchanged) with an adjustable threshold.
- **Swipe** — drag a divider to reveal Old vs New side by side.

### Markup tools
- Shapes: rectangle, circle, revision **cloud**, highlight, line, arrow, pen, polyline, polygon.
- Annotations: text, callout, stamps (APPROVED / REJECTED / …) and custom stamps, photo attachments.
- **Measurement**: length and area tools with a configurable scale (px / mm / m / ft / in).
- Layers (Architect / Contractor / Engineer / Coordination Review), color and line-width control.
- Markup list panel, undo, clear, select & delete.
- Works with mouse **and touch** (tablets / phones).

### Export
- **Export Page / Export All** to a marked-up PDF.
- **Batch All** — diff every page and export to a single PDF.
- **CSV** — Bluebeam-style markup summary.

### Single-PDF mode
Drop one PDF to mark it up without comparing.

## Usage

Just open `index.html` in a modern browser (Chrome, Edge, Firefox, Safari).
You can also publish it with **GitHub Pages** and use it online.

> ⚠️ The app loads [pdf.js](https://mozilla.github.io/pdf.js/) and [jsPDF](https://github.com/parallax/jsPDF) from a CDN, so an internet connection is required the first time / for each session.

## Privacy

All PDF processing happens **entirely in your browser**. No file is ever uploaded to any server.

## License

© Dang Quoc Truong (DQT). All rights reserved.
