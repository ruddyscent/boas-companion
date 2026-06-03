# Repository Instructions

## Project Scope

This repository contains original companion notes and solution writeups for
M. L. Boas, *Mathematical Methods in the Physical Sciences*, 3rd edition.

- Keep solution prose original. Do not copy full textbook problem statements,
  tables, figures, or other Wiley-owned material.
- Refer to exercises by chapter, section, and problem number instead of
  reproducing the source text.
- Match the existing `ch01/` style: clear English explanations, compact
  derivations, and enough context for the solution to stand on its own.

## Chapter 1 File Pattern

- Use `ch01/secNN.ipynb` for every Chapter 1 section, including prose-only
  sections.
- Keep section numbers zero-padded in filenames, for example
  `sec01.ipynb` and `sec14.ipynb`.
- Do not add new `*-solutions.md` or `*-solutions.ipynb` files under `ch01/`.

## Notebook Solution Format

- Start each notebook with a markdown title cell containing exactly one H1:

  ```md
  # 1-N. Section Title
  ```

- For a section with no assigned problems, use this minimal format:

  ```md
  # 1-N. No Assigned Problems

  This section has no problems in the textbook, so there are no solutions to list here.
  ```

- Write each exercise as an H3:

  ```md
  ### Problem K. Short Descriptive Title
  ```

- Use H2 headings only to group ranges of related problems, as in
  `## A. Comparison Test: Problems 1 through 6`.
- Use H4 headings for named subparts inside a problem, theorem references, or
  book equation references, for example `#### (13.2) The Series for $\cos x$`.
- Short blockquote notes at the top of a section are fine when they summarize
  the recurring method used in the section.

## Math and Prose Style

- Use inline LaTeX with `$...$` and display math with `$$...$$`.
- Put display equations on their own lines with blank lines around them.
- Show the main derivation before the conclusion. Prefer named tests and
  standard facts when appropriate: ratio test, integral test, comparison test,
  alternating series test, telescoping series, and so on.
- Use `\boxed{...}` sparingly for important final formulas or limits.
- For convergence problems, state the final classification or interval
  explicitly.
- For numerical answers, include approximations with `\approx` and include
  units or currency when relevant.
- Keep paragraphs short and direct. Avoid decorative exposition.

## Code Cell Style

- Use code cells only for numerical checks, symbolic or computational
  verification, and plots.
- Prefer small, readable Python snippets. Existing notebooks use standard
  library `math` and `matplotlib.pyplot` for most checks and plots.
- Keep notebook diffs clean. The pre-commit hook runs `nbdev-clean`; run it or
  `pre-commit run --all-files` before committing notebook edits.

## Development Notes

- JupyterLab can be started with `docker compose up`; see `README.md` for the
  local URL and token conventions.
- The project uses `uv` for dev tooling setup and `pre-commit` for notebook
  cleanup.
