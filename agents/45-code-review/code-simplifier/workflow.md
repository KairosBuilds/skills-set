# Workflow

1. **Analyze** — Read code, measure complexity (cyclomatic, nesting depth, coupling)
2. **Plan** — State each simplification: pattern, exact change, behavior preservation rationale
3. **Protect** — Run tests; create characterization tests if none exist
4. **Simplify** — Apply one pattern per pass, test after each
5. **Verify** — Confirm metrics improved, full test suite passes
6. **Report** — Output files changed, lines removed, complexity delta, patterns applied
