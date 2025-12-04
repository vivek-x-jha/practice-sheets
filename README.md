# Practice Sheets

Curated LaTeX worksheets for math practice by subject.

## Layout
- `algebra/`: Proportional-relationships assessments and related Algebra I material.
- `algebra2/`: Algebra II practice (polynomials, radicals, quadratics, etc.).
- `arithmetic/`: Fraction practice sheets.
- `teaser/`: Short topical teasers.
- Builds live in each subject’s `build/` folder; sources are under `src/`.

## Building
Use `latexmk` (preferred for builds/cleanup):
- Algebra: `latexmk -pdf -f -output-directory=algebra/build algebra/src/<file>.tex`
- Algebra2: `latexmk -pdf -f -output-directory=algebra2/build algebra2/src/<file>.tex`
- Arithmetic: `latexmk -pdf -f -output-directory=arithmetic/build arithmetic/src/<file>.tex`
- Teasers: `latexmk -pdf -f -output-directory=teaser/build teaser/src/<file>.tex`

## Cleaning
Preserve PDFs; remove auxiliary files with:
- `latexmk -c -output-directory=algebra/build algebra/src/<file>.tex`
- `latexmk -c -output-directory=algebra2/build algebra2/src/<file>.tex`
- `latexmk -c -output-directory=arithmetic/build arithmetic/src/<file>.tex`
- `latexmk -c -output-directory=teaser/build teaser/src/<file>.tex`

## Guidelines
See `AGENTS.md` for subject-specific instructions, problem counts, and formatting conventions. Always consult it before adding or editing sheets.
