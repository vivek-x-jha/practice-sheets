# Agent Memory

Durable practice-sheets facts for future agent sessions.

## Facts

- Last verified: 2026-07-02 from `README.md` and `AGENTS.md`.
- The repo contains curated LaTeX worksheets by subject: `algebra`, `algebra2`, `arithmetic`, `calculus`, `cheatsheets`, `geometry`, and `teasers`.
- Sources live under each subject's `src/`; built PDFs live under that subject's `build/`.
- After a successful `latexmk -pdf -f ...` build, immediately run the matching `latexmk -c ...` cleanup and verify the PDF remains.
- `AGENTS.md` contains the subject-specific worksheet rules; read it before generating or revising sheets.
