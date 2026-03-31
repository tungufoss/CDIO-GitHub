# CDIO Implementation Paper
## Using Pull Requests to Make Collaboration Visible in CDIO Project-Based Courses

This repository contains the source and supporting materials for a CDIO Implementation paper accepted with minor changes for the 22nd International CDIO Conference (2026).

**Title:**
Using Pull Requests to Make Collaboration Visible in CDIO Project-Based Courses

**Author:**
Helga Ingimundardottir
Assistant Professor of Industrial Engineering
University of Iceland

---

## Overview

This paper presents a CDIO implementation case describing the use of GitHub Classroom as collaboration and assessment infrastructure in industrial engineering undergraduate and mixed undergraduate/graduate courses.

The implementation addresses challenges common in team-based, open-ended, data-intensive project courses, including visibility of individual contribution, quality of collaboration, responsiveness to feedback, and reproducibility of results. Rather than treating GitHub as a programming topic, the platform is framed as a professional collaboration environment in which assessment is anchored to observable artifacts.

The core design centers on pull requests (PRs) as the primary unit of feedback and assessment. Students are required to author or co-author PRs, participate in substantive peer review with required approvals prior to merge, and respond explicitly to instructor comments within PR threads. Assessment emphasizes review quality, responsiveness to feedback, documentation and handover, and visible individual participation within collective work.

An early design using separate repositories per project cycle resulted in repeated onboarding, context loss, and high instructional overhead. The redesigned implementation adopts one persistent repository per team across the semester, enabling cumulative iteration, traceability, and efficient capstone evaluation. To reduce cognitive load during complex project work, instruction in GitHub collaboration practices is relocated to a prerequisite Information Engineering course, allowing later courses (such as Business Intelligence) to use the tool naturally without concurrent tool training.

The contribution is framed as an implementation and design paper, focusing on design decisions, trade-offs, assessment mechanisms, and transferability rather than learning-effect claims.

---

## Alignment with CDIO Standards

The implementation primarily addresses:

- CDIO Standard 7: Integrated Learning Experiences
- CDIO Standard 8: Active Learning
- CDIO Standard 11: Learning Assessment

with partial alignment to CDIO Standard 5: Design-Implement Experiences.

---

## Repository Contents

- `cdio2026-HelgaIngim-GitHub.tex`
  -> Main LaTeX source file (inputs `include/body.tex`, `include/stakeholders.tikz`, and `include/rubric.tex`)

- `include/body.tex`
  -> Paper body (sections and content)

- `include/stakeholders.tikz`
  -> Workflow diagram figure

- `include/rubric.tex`
  -> Rubric table

- `references.bib`
  -> BibLaTeX references

- `cdio.cls`
  -> CDIO conference class file

- `cdio2026-HelgaIngim-GitHub.pdf`
  -> Latest compiled paper PDF

- `REVIEWS.md`, `REVIEWS.pdf`
  -> Acceptance letter and reviewer comments

- `REVISION.md`, `REVISION.pdf`
  -> Response to reviewers

- `include/by-nc-nd.pdf`
  -> License figure used in the paper

---

## Build Information

The paper is compiled using LaTeX with the official `cdio.cls` class file and BibLaTeX (biber backend).

To compile locally:

```bash
xelatex cdio2026-HelgaIngim-GitHub.tex
biber cdio2026-HelgaIngim-GitHub
xelatex cdio2026-HelgaIngim-GitHub.tex
xelatex cdio2026-HelgaIngim-GitHub.tex
```
