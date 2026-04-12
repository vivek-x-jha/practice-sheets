# Practice Sheets

Curated LaTeX worksheets for math practice by subject.

## Tooling Notes
- For shell-based file and directory discovery in this repo, prefer `fd` over `find` when `fd` is available. Use `find` as a fallback or when a specific `find` feature is needed.

## Layout
- `algebra/`: Proportional-relationships assessments and related Algebra I material.
- `algebra2/`: Algebra II practice (polynomials, logarithms, rational functions, conics, polar coordinates, complex numbers in polar form, trig review including unit-circle values/inverse trig/triangle solving/graphing, series, and review sets).
- `arithmetic/`: Arithmetic and pre-algebra practice sheets.
- `calculus/`: Calculus AB-style practice (limits, derivative rules and definitions, integrals, washer/shell volume problems, particle motion, exponential/logistic/Newton models, and review sets).
- `cheatsheets/`: Compact reference sheets and formula summaries by topic.
- `geometry/`: Geometry and trigonometry practice (applications, Law of Sines/Cosines, and proof work).
- `teasers/`: Short topical teaser/problem sets.
- Builds live in each subject’s `build/` folder; sources are under `src/`.

## Building
Use `latexmk` (preferred for builds/cleanup):
- Algebra: `latexmk -pdf -f -output-directory=algebra/build algebra/src/<file>.tex`
- Algebra2: `latexmk -pdf -f -output-directory=algebra2/build algebra2/src/<file>.tex`
- Arithmetic: `latexmk -pdf -f -output-directory=arithmetic/build arithmetic/src/<file>.tex`
- Calculus: `latexmk -pdf -f -output-directory=calculus/build calculus/src/<file>.tex`
- Cheatsheets: `latexmk -pdf -f -output-directory=cheatsheets/build cheatsheets/src/<file>.tex`
- Geometry: `latexmk -pdf -f -output-directory=geometry/build geometry/src/<file>.tex`
- Teasers: `latexmk -pdf -f -output-directory=teasers/build teasers/src/<file>.tex`

## Cleaning
Preserve PDFs; remove auxiliary files with:
- `latexmk -c -output-directory=algebra/build algebra/src/<file>.tex`
- `latexmk -c -output-directory=algebra2/build algebra2/src/<file>.tex`
- `latexmk -c -output-directory=arithmetic/build arithmetic/src/<file>.tex`
- `latexmk -c -output-directory=calculus/build calculus/src/<file>.tex`
- `latexmk -c -output-directory=cheatsheets/build cheatsheets/src/<file>.tex`
- `latexmk -c -output-directory=geometry/build geometry/src/<file>.tex`
- `latexmk -c -output-directory=teasers/build teasers/src/<file>.tex`

## Guidelines
See `AGENTS.md` for subject-specific instructions, problem counts, and formatting conventions. Always consult it before adding or editing sheets.
