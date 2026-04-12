# General Worksheet Guidelines

- Maintain consistent LaTeX formatting with the existing sheets in each subject's `src/` folder, and build PDFs to that subject's `build/` folder.
- Include a clear instructions section with timing and answer-format expectations when that fits the worksheet type.
- Avoid giving hints or descriptive labels in problem statements unless a subject-specific rule says otherwise.
- State when exact form is expected; otherwise specify any rounding requirement clearly.

# Algebra2 Worksheet Guidelines

- Default to 12 problems unless otherwise specified; include an instructions section with timing and answer-format expectations.
- Focus on challenging Algebra II topics: rational root theorem, factoring (including quartics), polynomial long/synthetic division, complex roots and conjugate pairs, complex arithmetic, polar coordinates and conversions, De Moivre's formula, unit-circle trig values, inverse trig values, graphing the six trig functions, triangle area, solving triangles with the Law of Sines and Law of Cosines, vertex/maximum-minimum analysis of quadratics, logarithmic/exponential equations, rational functions, conic sections, finite/infinite series, and applied revenue/price optimization word problems.
- Present problems concisely and allow multi-part items when useful (e.g., list possible roots, find one, factor fully).
- Use exact forms over decimals.

# Algebra Worksheet Guidelines (Proportional Relationships Unit)

- Target 30-minute assessments that split focus: half on solving linear and quadratic equations (basic factoring, pure quadratics with only quadratic and constant terms, and quadratic formula) and half on proportional relationships.
- Use the unit framing: “Our next unit will be Proportional Relationships. This unit is a combination of work from Singapore Math (Chapter 5) and Open Up Resources (Units 1-3). The standards-based score for both units will be assessed by a variety of key assignments, Exit Tickets, assessments, and possible performance tasks.”

# Arithmetic Worksheet Guidelines

- Cover core fraction skills: addition, subtraction, multiplication, division, and mixed numbers; include occasional challenge problems that combine operations.
- Keep layout simple with grouped sections for each operation and total problem count aligned with the current arithmetic templates.
- Use answer-format directions like improper fractions when relevant.

# Calculus Worksheet Guidelines

- Focus on core Calculus AB topics currently in this repo: limits, derivative definitions and rules, tangent lines, definite integrals, Riemann sums, numerical integration, washer/shell volume problems, particle motion, and first-order differential-equation models such as exponential growth/decay, Newton's law of cooling, and logistic growth.
- Keep problem statements concise and assessment-style; include multi-part items when appropriate.

# Geometry Worksheet Guidelines

- Emphasize application problems with diagrams/contexts when relevant, including right-triangle trig, Law of Sines/Cosines, and proof/identity practice.
- Keep the worksheet style consistent with existing geometry assessments and practice sheets.

# Teaser Worksheet Guidelines

- Keep problems short, puzzle-like, and reasoning-focused.
- Prefer elegant number sense, divisibility, pattern, and logic prompts suitable for enrichment.

# Build and Clean Commands

- Build (Algebra): `latexmk -pdf -f -output-directory=algebra/build algebra/src/<file>.tex`
- Clean (Algebra): `latexmk -c -output-directory=algebra/build algebra/src/<file>.tex`
- Build (Algebra2): `latexmk -pdf -f -output-directory=algebra2/build algebra2/src/<file>.tex`
- Clean (Algebra2): `latexmk -c -output-directory=algebra2/build algebra2/src/<file>.tex`
- Build (Arithmetic): `latexmk -pdf -f -output-directory=arithmetic/build arithmetic/src/<file>.tex`
- Clean (Arithmetic): `latexmk -c -output-directory=arithmetic/build arithmetic/src/<file>.tex`
- Build (Calculus): `latexmk -pdf -f -output-directory=calculus/build calculus/src/<file>.tex`
- Clean (Calculus): `latexmk -c -output-directory=calculus/build calculus/src/<file>.tex`
- Build (Geometry): `latexmk -pdf -f -output-directory=geometry/build geometry/src/<file>.tex`
- Clean (Geometry): `latexmk -c -output-directory=geometry/build geometry/src/<file>.tex`
- Build (Teasers): `latexmk -pdf -f -output-directory=teasers/build teasers/src/<file>.tex`
- Clean (Teasers): `latexmk -c -output-directory=teasers/build teasers/src/<file>.tex`
- Prefer `latexmk -c` for cleanup; do not delete PDFs when cleaning build artifacts.

# Build Hook

- After any successful LaTeX build using `latexmk -pdf -f ...`, immediately run cleanup for that same file as part of the default workflow.
- Do not ask the user whether cleanup should happen after a successful build unless they explicitly request otherwise.
- Do not run build and clean in parallel. Build first, then clean, then verify that the PDF remains in the appropriate `build/` folder.
- If `latexmk -c` leaves auxiliary artifacts behind for a specific file, remove only that file's non-PDF build artifacts directly and verify that only the PDF remains.
