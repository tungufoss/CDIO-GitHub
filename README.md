
# CDIO Implementation Paper  
## Pull Requests as Assessment Infrastructure in CDIO Project Courses

This repository contains the source files for a **CDIO Implementation Paper** submitted to the **22nd International CDIO Conference (2026)**.

**Title:**  
Pull Requests as Assessment Infrastructure in CDIO Project Courses

**Author:**  
Helga Ingimundardóttir  
Assistant Professor of Industrial Engineering  
University of Iceland

---

## Overview

This paper presents a **CDIO Implementation case** describing the use of **GitHub Classroom as collaboration and assessment infrastructure** in industrial engineering undergraduate and mixed undergraduate/graduate courses.

The implementation addresses challenges common in **team‑based, open‑ended, data‑intensive project courses**, including visibility of individual contribution, quality of collaboration, responsiveness to feedback, and reproducibility of results. Rather than treating GitHub as a programming topic, the platform is framed as a **professional collaboration environment** in which assessment is anchored to observable artifacts.

The core design centers on **pull requests (PRs) as the primary unit of feedback and assessment**. Students are required to author or co‑author PRs, participate in substantive peer review with required approvals prior to merge, and respond explicitly to instructor comments within PR threads. Assessment emphasizes review quality, responsiveness to feedback, documentation and handover, and visible individual participation within collective work.

An early design using separate repositories per project cycle resulted in repeated onboarding, context loss, and high instructional overhead. The redesigned implementation adopts **one persistent repository per team across the semester**, enabling cumulative iteration, traceability, and efficient capstone evaluation. To reduce cognitive load during complex project work, instruction in GitHub collaboration practices is relocated to a **prerequisite Information Engineering course**, allowing later courses—such as Business Intelligence—to use the tool naturally without concurrent tool training.

The contribution is framed as an **implementation and design paper**, focusing on design decisions, trade‑offs, assessment mechanisms, and transferability rather than learning‑effect claims.

---

## Alignment with CDIO Standards

The implementation primarily addresses:

- **CDIO Standard 7** – Integrated Learning Experiences  
- **CDIO Standard 8** – Active Learning  
- **CDIO Standard 11** – Learning Assessment  

with partial alignment to **CDIO Standard 5** – Design–Implement Experiences.

---

## Repository Contents

- `cdio2026-HelgaIngim-GitHub.tex`  
  → Main LaTeX source file

- `body.tex`  
  → Paper body (sections and content)

- `references.bib`  
  → BibTeX references

- `graphics/`  
  → Figures used in the paper

---

## Build Information

The paper is compiled using **LaTeX** with the official `cdio.cls` class file provided by the CDIO Conference.

To compile locally:

```bash
pdflatex cdio2026-HelgaIngim-GitHub.tex
bibtex cdio2026-HelgaIngim-GitHub
pdflatex cdio2026-HelgaIngim-GitHub.tex
pdflatex cdio2026-HelgaIngim-GitHub.tex
```