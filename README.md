# Hidden States and Unassigned Work

Exact models and decisive measurements for higher-order ODEs

[Read the PDF](hidden-states-and-unassigned-work.pdf) · [Read the manuscript](hidden-states-and-unassigned-work.md)

Hob Nilre & Bo C. Herlin — 2026-09-26

This companion develops eighteen questions about physical realization, preparation, identification, collision release, switching, and signed work. It distinguishes exact model results from the physical transfers and measurement questions that remain open. All worked values follow from closed forms; the project contains no numerical simulations or measured data.

The related article is [*Third- and Higher-Order ODEs*](https://github.com/hobnilre/physics-ode-3rd-deg/blob/main/third-and-higher-order-odes.pdf).

Build with `make pdf`. Requirements: GNU Make, Pandoc, XeLaTeX, TikZ/PGFPlots, circuitikz, and the TeX Gyre Termes, Heros, Cursor and Termes Math fonts. `make -B pdf` rebuilds all figures and the article. `make clean` removes only the local `build/` directory and preserves the deliverable PDFs.

Notation, scales, and signs are in [notes/conventions.md](notes/conventions.md). The separate scope and verification record is in [notes/problem-audit.md](notes/problem-audit.md). Figures are standalone LaTeX documents and their PDFs are included. Build intermediates are ignored. No remote or commit is created.
