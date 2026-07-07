---
name: incremental-implementation
description: Implements features and changes in small, safe, mergeable increments. Covers slicing work, maintaining a green build, making each increment independently valuable, and getting early feedback. Use when implementing any non-trivial feature or change. Not for exploratory work or research.
license: MIT
compatibility: opencode
metadata:
  author: "Prateek"
  version: "1.0.0"
  domain: workflow
  triggers: implement, build feature, add functionality, develop, coding, start implementation
  role: specialist
  scope: development
  output-format: code
  related-skills: design-thinker, test-master, code-reviewer, definition-of-done
---

# Incremental Implementation

Implement features in small, safe, mergeable increments. Each increment must leave the codebase in a working state.

## Core Rules

1. **Green at every step** — The build must pass after each increment. Never leave the tree red.
2. **Every increment is mergeable** — If you stopped after any single increment, the partial feature would be harmless or gated behind a flag.
3. **Smallest meaningful slice** — Each increment adds one atomic unit of value: a type, a function, a test, a route, a component.
4. **Test alongside code** — Write tests in the same increment as the code they cover, not after.
5. **Commit after each increment** — Each passing state gets a commit with a clear message.

## Slicing Strategy

Slice work along these dimensions (in order of preference):

1. **Data first** — Types, schemas, models, validators before logic
2. **Core path first** — Happy path before edge cases and error handling
3. **Test first** — Write the test for the slice, watch it fail, make it pass
4. **Read before write** — Read operations before write/mutate operations
5. **Public before private** — Interface/API contract before implementation details
6. **Backend before frontend** — API/service layer before UI (for full-stack work)

### Example: User Profile Feature

```
Increment 1: User type/interface + validation
Increment 2: Get profile endpoint + test
Increment 3: Update profile endpoint + test
Increment 4: Profile page component (read-only)
Increment 5: Profile edit form UI
Increment 6: Error states, edge cases, polish
```

## Workflow

1. **Slice** — Break the feature into increments. Show the plan to the user and confirm the first increment.
2. **Implement one increment** — Write tests. Implement code. Run tests. Ensure green.
3. **Review increment** — Check diff scope: does it only touch what this increment needs?
4. **Commit** — Descriptive message following project convention.
5. **Repeat** — Move to the next increment. Re-slice if new understanding emerges.

## Anti-Patterns

| Anti-Pattern | Problem | Better Approach |
|---|---|---|
| One massive branch | Unmergeable for weeks, merge hell | Slice into daily increments |
| Test after implementation | Tests get skipped or rushed | Test in same increment as code |
| Edge cases in first increment | Core path blocked by rare conditions | Happy path first, edges later |
| Frontend before backend | Mocks that don't match reality | API contract first |

## Output

```
Increment: N of M
Files changed: [list]
Tests: [pass/fail]
Status: green/blocked
Next increment: [description]
```
