# PlotBench

Publication-quality graphs — grouped bars, line/XY, and dose–response — built entirely in the browser. It's a free, single-file alternative to commercial software for routine lab figures: no account, no install, no licence, and **your data never leaves your machine** (everything runs client-side). The whole app is one `index.html` file you can open locally, keep on a shared drive, or host so the whole lab uses the same link.

## Features

- **Grouped bars, line/XY, and combined dose–response** figures, with SD / SEM / 95% CI error bars and optional individual-point overlay.
- **4PL curve fitting** with EC50, Hill slope, R², constrainable Top/Bottom, optional **1/Y² weighting**, and **profile-likelihood confidence intervals**.
- **Combined dose–response figures**: a bars panel beside a curve panel on one shared, optionally **broken (discontinuous) Y-axis** that auto-detects the gap in your data.
- **Multi-panel layouts**: arrange several figures into one labelled composite (A, B, C…).
- **Export** to vector **SVG**, high-resolution **PNG**, and vector **PDF**; **save/open** an entire project (all figures + layout) as one JSON file.
- Paste data straight from a spreadsheet. Built-in **? Guide** explains the whole workflow.

## Use it

Open `index.html` in any modern browser — that's it. Click **? Guide** (top right) for a walkthrough, or **Dose–response → Load worked example** for a synthetic example you can edit.

## Host it on GitHub Pages

1. Put `index.html` in the root of a **public** repository (free Pages requires a public repo).
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Set the branch to `main` and the folder to `/ (root)`, then **Save**.
5. Wait a minute or two; your site appears at `https://<username>.github.io/<repo>/`.

The app is a static site that runs entirely in the visitor's browser, so it sits comfortably within GitHub Pages' limits (1 GB site size, 100 GB/month soft bandwidth) even with a whole lab using it.

## Privacy

All computation happens locally in the browser. No data is uploaded, stored, or transmitted anywhere.

## Bundled libraries

PDF export uses [jsPDF](https://github.com/parallax/jsPDF) and [svg2pdf.js](https://github.com/yWorks/svg2pdf.js) (both MIT-licensed), inlined so the tool works fully offline.
