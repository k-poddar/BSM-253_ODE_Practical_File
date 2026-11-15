# $\LaTeX$ Typesetting — BSM-253 Ordinary Differential Equations Lab Practical File

Complete **$\LaTeX$ typesetting and modular document design** for my **BSM-253 (Ordinary Differential Equations Lab)** practical file as a 2nd-year Mathematics student at University School of Basic and Applied Sciences, Guru Gobind Singh Indraprastha University.

Built from scratch in VS Code, this repository demonstrates clean mathematical formatting, syntax-highlighted code blocks, and automated multi-file PDF assembly.

> **📄 [View Final Typeset PDF (`main.pdf`)](./main.pdf)**

---

## $\LaTeX$ Typesetting & Formatting Highlights

* **Multi-File Document Assembly (`main.tex`):** Uses `pdfpages` and `pgffor` (`\foreach`) loops to merge 15 standalone documents (cover page, index, and 13 practical reports) with blank separator pages (`\thispagestyle{empty}`) for clean double-sided printing.
* **Mathematical Equations & Derivations:** Typeset first- and higher-order differential equations, coupled systems, piecewise functions (`cases`), and multi-step derivations using `amsmath` and `amssymb`.
* **Custom Title Page & Index Tables:** Designed an institutional cover sheet (`array`) and a structured, auto-adjusting index table (`tabularx`, `booktabs`) with columns for serial numbers, practical aims, dates, and signatures.
* **Framed Code Listings:** Configured `matlab-prettifier` and `listings` with line-wrapping and editor-style framing so computational scripts sit cleanly alongside mathematical theory and plots.
* **Clean Project Organization:** Separated source `.tex` files and figures (`\graphicspath`) with `.gitignore` rules to keep temporary compiler artifacts out of the repository.

---

## Repository Structure

```text
├── main.tex       # Master file for merging all sections
├── main.pdf       # Final typeset practical file
├── tex/           # Individual LaTeX source files (cover, index, P1–P13)
└── figures/       # High-resolution plots and university logo
```

---

## Contents Typeset

* **Front Matter:** Institutional cover page and practical index.
* **Practicals 1–5:** Solution families of first-, second-, third-, and fourth-order ODEs, and coupled linear systems.
* **Practicals 6–9:** Exponential growth and decay, constant and seasonal lake pollution, piecewise Heaviside cold-pill dosage models, and logistic growth with harvesting.
* **Practicals 10–13:** Lotka–Volterra predator–prey models, density dependence, SIR influenza epidemic models, and Lanchester battle models.

---

## How to Compile Locally

1. Compile the individual `.tex` files inside `tex/` (`cover.tex`, `index.tex`, and `P1.tex`–`P13.tex`) using `pdflatex` (or LaTeX Workshop in VS Code) to generate their standalone PDFs in `tex/`.
2. Compile `main.tex` in the root directory to produce the merged **`main.pdf`**:
   ```bash
   pdflatex main.tex
   ```

---

## About Me

Hello, I am **Kavya Poddar** — a 2nd-year **B.Sc. Mathematics** student with a minor in **Quantum Information** at USBAS, GGSIPU.

This project reflects my ongoing practice in using $\LaTeX$ to format mathematical work and code clearly and neatly.