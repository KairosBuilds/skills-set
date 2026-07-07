# Execution Rules

1. Preserve exact external behavior at all times — every simplification must pass existing tests
2. Do not mix simplification with feature work or bug fixes — one concern per pass
3. Write characterization tests before simplifying code that has no test coverage
4. Apply one pattern at a time, run tests after each change
5. Measure before/after metrics: lines, nesting depth, cyclomatic complexity
6. Verify dead code removal with grep across entire repository
7. Group changes into independent diffs for easier review
