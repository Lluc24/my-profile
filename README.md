# Professional Documents | Lluc Santamaria Riba

This repository serves as a central archive for my professional documentation. It houses the complete record of my academic background, professional experience, and contact information in Markdown, alongside the LaTeX source code and compiled assets for my Curriculum Vitae and professional business card.

## Source of Truth

[`BACKGROUND.md`](BACKGROUND.md) is the canonical, human- and machine-readable record of my full professional profile — experience, education, projects, awards, and volunteering. The CV and business card are curated, derived views of this content. When information changes, `BACKGROUND.md` is updated first; the LaTeX documents are then regenerated to match.

## Repository Contents

| Path | Description |
| --- | --- |
| [`BACKGROUND.md`](BACKGROUND.md) | Full professional background (single source of truth). |
| [`cv/`](cv) | Curriculum Vitae LaTeX source (`Lluc_Santamaria_CV.tex`) and compiled PDF. |
| [`business_card/`](business_card) | Business card LaTeX source (`card.tex`), compiled PDF, and QR code asset. |

You can view the latest compiled versions directly here:
- [View Curriculum Vitae (PDF)](cv/Lluc_Santamaria_CV.pdf)
- [View Business Card (PDF)](business_card/card.pdf)

## Build Instructions

To compile these documents from source, a standard TeX distribution (such as TeX Live or MiKTeX) is required. Please note that the LaTeX source files require two consecutive compilation passes to correctly resolve page numbering and cross-references.

**Compiling the CV:**

```bash
cd cv
pdflatex Lluc_Santamaria_CV.tex
pdflatex Lluc_Santamaria_CV.tex
```

**Compiling the Business Card:**

```bash
cd business_card
pdflatex card.tex
```

## Usage and License

The contents of this repository are provided primarily for reference, verification, and recruitment purposes. While the LaTeX formatting and structure may be referenced for educational purposes, the personal data and specific content within these documents remain the intellectual property of the author. Please do not redistribute, modify, or reuse the personal details contained herein without explicit permission.