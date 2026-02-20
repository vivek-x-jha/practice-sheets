# Practice Sheets

Curated LaTeX worksheets for math practice by subject.

## Layout
- `algebra/`: Proportional-relationships assessments and related Algebra I material.
- `algebra2/`: Algebra II practice (polynomials, logarithms, rational functions, conics, series, and review sets).
- `arithmetic/`: Arithmetic and pre-algebra practice sheets.
- `calculus/`: Calculus AB-style practice (limits, derivatives, integrals, particle motion, and review sets).
- `geometry/`: Geometry and trigonometry practice (applications, Law of Sines/Cosines, and proof work).
- `teasers/`: Short topical teaser/problem sets.
- Builds live in each subject’s `build/` folder; sources are under `src/`.

## Building
Use `latexmk` (preferred for builds/cleanup):
- Algebra: `latexmk -pdf -f -output-directory=algebra/build algebra/src/<file>.tex`
- Algebra2: `latexmk -pdf -f -output-directory=algebra2/build algebra2/src/<file>.tex`
- Arithmetic: `latexmk -pdf -f -output-directory=arithmetic/build arithmetic/src/<file>.tex`
- Calculus: `latexmk -pdf -f -output-directory=calculus/build calculus/src/<file>.tex`
- Geometry: `latexmk -pdf -f -output-directory=geometry/build geometry/src/<file>.tex`
- Teasers: `latexmk -pdf -f -output-directory=teasers/build teasers/src/<file>.tex`

## Cleaning
Preserve PDFs; remove auxiliary files with:
- `latexmk -c -output-directory=algebra/build algebra/src/<file>.tex`
- `latexmk -c -output-directory=algebra2/build algebra2/src/<file>.tex`
- `latexmk -c -output-directory=arithmetic/build arithmetic/src/<file>.tex`
- `latexmk -c -output-directory=calculus/build calculus/src/<file>.tex`
- `latexmk -c -output-directory=geometry/build geometry/src/<file>.tex`
- `latexmk -c -output-directory=teasers/build teasers/src/<file>.tex`

## Guidelines
See `AGENTS.md` for subject-specific instructions, problem counts, and formatting conventions. Always consult it before adding or editing sheets.
