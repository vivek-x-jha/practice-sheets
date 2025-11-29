# Algebra2 Worksheet Guidelines

- Default to 12 problems unless otherwise specified; include an instructions section with timing and answer-format expectations.
- Focus on challenging Algebra II topics: rational root theorem, factoring (including quartics), polynomial long/synthetic division, complex roots and conjugate pairs, complex arithmetic, vertex/maximum-minimum analysis of quadratics, and applied revenue/price optimization word problems.
- Avoid giving hints or descriptive labels in problem statements; present problems concisely and allow multi-part items when useful (e.g., list possible roots, find one, factor fully).
- Use exact forms over decimals; state when exact form is expected.
- Maintain formatting consistent with sheets under `algebra2/src`; build PDFs to `algebra2/build`.

# Algebra Worksheet Guidelines (Proportional Relationships Unit)

- Target 30-minute assessments that split focus: half on solving linear and quadratic equations (basic factoring, pure quadratics with only quadratic and constant terms, and quadratic formula) and half on proportional relationships.
- Use the unit framing: “Our next unit will be Proportional Relationships. This unit is a combination of work from Singapore Math (Chapter 5) and Open Up Resources (Units 1-3). The standards-based score for both units will be assessed by a variety of key assignments, Exit Tickets, assessments, and possible performance tasks.”
- Keep instructions clear about timing and exact-form expectations; avoid hinting in problem statements.
- Maintain LaTeX formatting with sheets under `algebra/src`; build PDFs to `algebra/build`.

# Arithmetic Worksheet Guidelines

- Use clear instructions about answer format (e.g., improper fractions) and time expectations.
- Cover core fraction skills: addition, subtraction, multiplication, division, and mixed numbers; include occasional challenge problems that combine operations.
- Keep layout simple with grouped sections for each operation and total problem count aligned with the current arithmetic templates.
- Maintain consistent LaTeX formatting with existing sheets under `arithmetic/src`, building PDFs to `arithmetic/build`.

# Build and Clean Commands

- Build (Algebra): `latexmk -pdf -f -output-directory=algebra/build algebra/src/<file>.tex`
- Clean (Algebra): `latexmk -c -output-directory=algebra/build algebra/src/<file>.tex`
- Build (Algebra2): `latexmk -pdf -f -output-directory=algebra2/build algebra2/src/<file>.tex`
- Clean (Algebra2): `latexmk -c -output-directory=algebra2/build algebra2/src/<file>.tex`
- Build (Arithmetic): `latexmk -pdf -f -output-directory=arithmetic/build arithmetic/src/<file>.tex`
- Clean (Arithmetic): `latexmk -c -output-directory=arithmetic/build arithmetic/src/<file>.tex`
- Prefer `latexmk -c` for cleanup; do not delete PDFs when cleaning build artifacts.
