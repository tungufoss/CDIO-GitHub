# CDIO Implementation Paper
## Using Pull Requests to Make Collaboration Visible in CDIO Project-Based Courses

**Author:** Helga Ingimundardóttir, Assistant Professor of Industrial Engineering, University of Iceland
**Event:** 22nd International CDIO Conference, June 24th, 2026

---

## Overview

This repository contains the paper source and the conference presentation for a CDIO Implementation paper accepted for the 22nd International CDIO Conference (2026).

The paper presents a case describing the use of GitHub Classroom as collaboration and assessment infrastructure in industrial engineering courses. Pull requests are the primary unit of feedback and assessment — making individual contribution, review quality, and responsiveness to feedback visible and assessable.

---

## Presentation (Quarto RevealJS)

The slides are built with [Quarto](https://quarto.org/) using a custom HI (University of Iceland) RevealJS theme.

To render:

```bash
quarto render slides.qmd
```

Output: `index.html`

### Structure

| Path | Description |
|------|-------------|
| `slides.qmd` | Main presentation source |
| `index.html` | Rendered presentation |
| `styles/colors.css` | HI brand colour variables |
| `styles/hi26-reveal.css` | Base HI RevealJS theme |
| `styles/cdio2026.css` | Conference-specific overrides |
| `styles/watermark-inline.css` | Draft watermark (disable for final) |
| `_extensions/card-enum/` | Lua filter: `.fa-card` and `.card-enum` layouts |
| `_extensions/hi-title/` | Lua filter: HI title slide shortcode |
| `_extensions/menti/` | Lua filter: Mentimeter embed shortcode |
| `_extensions/pause/` | Lua filter: animated pause shortcode |
| `partials/header-includes.inc` | Font Awesome + Jost font CDN links |
| `partials/body-after.inc` | Scripts injected after body |
| `partials/contact-card.html` | Reusable contact card HTML |
| `scripts/countdown.js` | Countdown timer script |
| `include/stakeholders.svg` | Inline SVG: Git workflow diagram |
| `include/vr2.jpg` | Photo used on contact slide |
| `img/hi/` | HI logos and favicon |

---

## Paper (LaTeX)

The paper is compiled with XeLaTeX and BibLaTeX (biber backend).

To compile:

```bash
xelatex cdio2026-HelgaIngim-GitHub.tex
biber cdio2026-HelgaIngim-GitHub
xelatex cdio2026-HelgaIngim-GitHub.tex
xelatex cdio2026-HelgaIngim-GitHub.tex
```

### Structure

| Path | Description |
|------|-------------|
| `cdio2026-HelgaIngim-GitHub.tex` | Main LaTeX source |
| `cdio2026-HelgaIngim-GitHub.pdf` | Compiled paper PDF |
| `cdio.cls` | CDIO conference class file |
| `references.bib` | BibLaTeX references |
| `include/body.tex` | Paper body |
| `include/rubric.tex` | Assessment rubric table |
| `include/stakeholders.tikz` | TikZ workflow diagram |
| `include/by-nc-nd.pdf` | CC BY-NC-ND licence figure |

---

## Review Materials

| Path | Description |
|------|-------------|
| `REVIEWS.md` / `REVIEWS.pdf` | Acceptance letter and reviewer comments |
| `REVISION.md` / `REVISION.pdf` | Response to reviewers |

---

## CDIO Standards Alignment

- **Standard 7** — Integrated Learning Experiences
- **Standard 8** — Active Learning
- **Standard 11** — Learning Assessment
- **Standard 5** — Design-Implement Experiences (partial)
