---
name: definition-of-done
description: Standing quality checklist that every change must clear before it counts as done. Covers correctness, quality, integration, documentation, and ship-readiness. Use as the final gate on any task, feature, or release. Complements acceptance criteria which vary per task.
license: MIT
compatibility: opencode
metadata:
  author: "Prateek"
  version: "1.0.0"
  domain: code-quality
  triggers: definition of done, done checklist, quality gate, is it ready, acceptance criteria
  role: standard
  scope: quality
  output-format: checklist
  related-skills: code-reviewer, test-master, security-reviewer, shipping-and-launch
---

# Definition of Done

A standing, project-wide bar that every change must clear before it counts as done. Unlike acceptance criteria, which vary per task, the Definition of Done is the same every time and answers "is this finished to our standard?"

## Definition of Done vs. Acceptance Criteria

| | Acceptance Criteria | Definition of Done |
|---|---|---|
| Scope | Specific to one task or spec | Applies to every increment |
| Changes | Different for each item | Fixed and reused |
| Answers | "Did we build this thing?" | "Is it ready?" |
| Owner | Defined when planning the task | Defined once for the project |
| Example | "User can reset password via email link" | "Tests pass, no regressions, docs updated" |

A task is done only when its acceptance criteria are met AND the standing Definition of Done is satisfied.

## The Standing Checklist

### Correctness
- All acceptance criteria for the task are met
- Code runs and behaves as intended, verified at runtime (not just compiled or typechecked)
- New behavior is covered by tests that fail without the change and pass with it
- Existing tests still pass; no regressions introduced
- Edge cases and error paths are handled, not just the happy path

### Quality
- Code reveals intent through naming and structure
- No duplicated business logic
- No dead code, debug output, or commented-out blocks left behind
- Changes are scoped to the task; no unrelated refactors snuck in
- Linting and formatting pass

### Integration
- Change works with the rest of the system, not just in isolation
- Database migrations, config changes, and feature flags are accounted for
- Backward compatibility considered for any public interface or API change

### Documentation
- Public interfaces, APIs, and user-facing behavior are documented
- Architectural decisions worth preserving are recorded
- Documentation describes the current state in timeless language

### Ship-readiness
- Security implications reviewed for untrusted input, auth, or data handling
- Observability in place for new critical paths (logs, metrics, traces)
- Rollback path exists for anything risky
- The human has reviewed and approved before merge or deploy

## How to Apply

- Per task: confirm Correctness and Quality sections before checking off
- Per feature: confirm Integration and Documentation before considering feature complete
- Per release: the full checklist is the floor; shipping-and-launch adds deploy-specific gates

## Red Flags

- "It's done, I just haven't run it yet": unverified work is not done
- "Tests pass" used as synonym for done while docs, regressions, or runtime verification are skipped
- A different bar applied depending on deadline pressure
- Acceptance criteria treated as the whole bar with no standing quality floor
- "Done" declared before human review on changes that need it
