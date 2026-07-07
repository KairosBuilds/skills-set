---
name: code-simplification
description: Reduces code complexity without changing behavior. Covers eliminating duplication, flattening conditionals, removing dead code, simplifying state, reducing coupling, and improving readability. Use when a codebase has grown complex, reviews flag readability issues, or cyclomatic complexity is high. Not for adding features or changing behavior.
license: MIT
compatibility: opencode
metadata:
  author: "Prateek"
  version: "1.0.0"
  domain: code-quality
  triggers: simplify, refactor, reduce complexity, clean up, technical debt, readability
  role: specialist
  scope: refactoring
  output-format: diff
  related-skills: code-reviewer, definition-of-done, staff-engineer-review
---

# Code Simplification

Reduce complexity without changing behavior. Every simplification must preserve the exact external behavior.

## Core Principles

1. **Preserve behavior** — Every refactor must pass existing tests. If no tests exist, add characterization tests before simplifying.
2. **One concern per pass** — Never mix simplification with feature work or bug fixes.
3. **Measurable improvement** — Each change should reduce a concrete metric: lines of code, nesting depth, number of conditionals, number of parameters, or coupling count.

## Simplification Patterns

### Eliminate Duplication
- Extract repeated expressions into named functions
- Unify similar data structures
- Replace copy-paste with loops or generics

### Flatten Conditionals
- Replace nested if/else with guard clauses (early return)
- Replace switch/if chains with lookup tables or polymorphism
- Combine related conditions into named predicates
- Replace flag parameters with separate functions

### Simplify State
- Replace mutable state with immutable data where possible
- Reduce number of state fields; derived state should be computed
- Replace boolean flags with enumerations or strategy objects

### Reduce Coupling
- Replace direct dependency with interface/abstraction
- Move unrelated logic out of a class or module
- Reduce parameter counts (introduce parameter object or builder)

### Simplify Data Flow
- Replace callbacks with async/await or promises
- Replace shared mutable state with explicit data passing
- Remove unused parameters from function signatures

### Remove Dead Code
- Delete unused functions, classes, imports, and variables (verify with grep)
- Remove commented-out code
- Remove unreachable branches
- Remove debug logging and dev-only code paths

## Workflow

1. **Analyze** — Identify complexity hotspots. Read the code. Measure: cyclomatic complexity, function length, nesting depth, coupling count.
2. **Plan** — For each simplification, state: (a) what pattern applies, (b) the exact change, (c) why it preserves behavior. Group into independent diffs.
3. **Protect** — Run tests before any change. Create characterization tests if none exist.
4. **Simplify** — Apply one pattern at a time. Run tests after each change.
5. **Verify** — Confirm metrics improved. Run full test suite.

## Output

```
Simplification Summary
- Files changed: N
- Lines removed: N
- Complexity reduced: X → Y
- Patterns applied: [list]
- Verification: [test command output]

Key changes:
1. [file:line] — [pattern applied]
2. [file:line] — [pattern applied]
```
