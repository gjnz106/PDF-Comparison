# PDF Compare — DQT

A single-file, browser-based tool to **compare two revisions of a PDF** and **mark up** drawings — no install, no server, everything runs locally in the browser.

> Author: Dang Quoc Truong (DQT)

## Features

### Compare modes
- **Overlay** — blend Old/New revisions with an opacity slider.
- **Pixel Diff** — colored difference map (red = removed, green = added, grey = unchanged) with an adjustable threshold, computed in a background **Web Worker** so the UI stays responsive on large PDFs.
- **Swipe** — drag a divider to reveal Old vs New side by side.

### Markup tools
- Shapes: rectangle, circle, revision **cloud**, highlight, line, arrow, pen, polyline, polygon.
- Annotations: text, callout, stamps (APPROVED / REJECTED / …) and custom stamps, photo attachments.
- **Measurement**: length and area tools with a configurable scale (px / mm / m / ft / in).
- Layers (Architect / Contractor / Engineer / Coordination Review), color and line-width control.
- Markup list panel, undo, clear, select & delete (with a visible selection frame on every markup type).
- Works with mouse **and touch** (tablets / phones); polyline / polygon / area have **Finish** & **Cancel** buttons so they can be completed without a double-click.

### Save & restore
- Markups are **auto-saved** to the browser (localStorage), keyed by the loaded file name(s), and restored automatically the next time you open the same files.
- **Save / Load** buttons export and import a portable `.mkup.json` file to move markups between machines.

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

---

## Also in this repo: `ifc-viewer.html`

`ifc-viewer.html` is a separate, self-contained prototype — **IFC Delta 3D**, a BIM
model-comparison UI built to the *Neutral + Charcoal v4* design system
(`design_handoff`). It implements the three-pane shell (header, versions sidebar,
3D viewport, properties panel), Field/Compare/Clash modes, the colorize legend,
opacity slider, search/issues/tree tabs, the SG (Safeguarding) validator dock, and
toast/popover/accordion interactions. Static UI prototype with sample data — open
the file directly in a browser. Requires internet for the Google Fonts
(Hanken Grotesk + JetBrains Mono).
