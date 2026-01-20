# Professional Documents | Lluc Santamaria Riba

This repository serves as a central archive for my professional documentation, authored and maintained in LaTeX. It currently houses the source code and compiled assets for my Curriculum Vitae and professional business card. These documents reflect my most current academic background, professional experience, and contact information.

## Repository Contents

The project is organized into two primary directories. The `cv` directory contains the source code for my Curriculum Vitae (`Lluc_Santamaria_CV.tex`) and the resulting PDF. The `business_card` directory contains the design and logic for my contact cards, including the necessary QR code assets.

You can view the latest compiled versions directly here:
- [View Curriculum Vitae (PDF)](cv/Lluc_Santamaria_CV.pdf)
- [View Business Card (PDF)](business_card/Lluc_Santamaria_card.pdf)

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
pdflatex Lluc_Santamaria_card.tex
```

## Usage and License

The contents of this repository are provided primarily for reference, verification, and recruitment purposes. While the LaTeX formatting and structure may be referenced for educational purposes, the personal data and specific content within these documents remain the intellectual property of the author. Please do not redistribute, modify, or reuse the personal details contained herein without explicit permission.