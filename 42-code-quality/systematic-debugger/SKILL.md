---
name: systematic-debugger
description: Finds root cause before applying fixes for errors, crashes, regressions, failing tests, and broken behavior. Systematic approach covering hypothesis-driven diagnosis, bisect, scope blast, and runtime evidence verification. Use for debugging errors, regressions, failing tests, or unexpected behavior. Not for code review or new features.
license: MIT
compatibility: opencode
metadata:
  author: "Prateek"
  version: "1.0.0"
  domain: code-quality
  triggers: debug, root cause, error, crash, regression, broken, not working, bug, investigate
  role: specialist
  scope: debugging
  output-format: analysis
  related-skills: debugger, debugging-wizard, code-reviewer
---

# Systematic Debugger

Finds root cause before applying any fix. A patch applied to a symptom creates a new bug somewhere else.

## Outcome Contract

- Outcome: root cause is identified before any fix is applied.
- Done when: one sentence explains the cause, every observed symptom fits it, and the fix or handoff is verified against a reproducible check.
- Evidence: source trace, repro command or UI path, logs or state, targeted test/build output.
- Output: root cause, fix or handoff, verification result, and any unswept sibling risks.

**Do not touch code until you can state the root cause in one sentence:**
> "I believe the root cause is [X] because [evidence]."

Name a specific file, function, line, or condition. If you cannot be that specific, you do not have a hypothesis yet.

## Hard Rules

- Same symptom after a fix is a hard stop. Re-read the execution path from scratch before touching code again.
- After three failed hypotheses, stop. Surface what was checked, ruled out, and what is unknown. Ask how to proceed.
- Verify before claiming. Never state versions, function names, or file locations from memory. Run commands first.
- Fix the cause, not the symptom. If the fix touches more than 5 files, pause and confirm scope.

## Bisect Mode

Activate when something used to work. Protect the user's worktree first. Define a non-interactive pass/fail test command before starting. Let bisect drive the commits; do not skip ahead. When bisect names the culprit, read only that diff to identify the specific line.

## Scope Blast Mode

Activate after fixing a root-cause pattern, before declaring the bug done. The same shape often hides in N other places.

1. Extract the pattern signature: specific function name, regex, API call, CSS selector, or input boundary.
2. `grep -rn <pattern>` across the repo (exclude generated dirs).
3. List every match. For each: same bug here? Pick fix / leave (explain why safe) / unsure (ask user).
4. Do not claim fixed until the blast report is in the output.

## Confirm or Discard

Run the one probe that would fail if the hypothesis were wrong. If evidence contradicts the hypothesis, discard it completely and re-orient.

## Runtime Evidence Ladder

1. Source trace: exact function, state transition, file, line, or condition
2. Deterministic repro: smallest command, fixture, or UI path
3. Logs/state/cache: runtime state proving the path was reached
4. Build/test: narrow test or build exercising the fix
5. Real runtime check: for UI/native/visual bugs, open and verify the result

## Regression Guard Rule

For any bug that recurred, the fix is not done until:
1. A regression test exists that fails on the unfixed code and passes on the fixed code.
2. The test lives in the project's test suite.
3. The commit message states why the bug recurred and why this fix prevents it.

## Output

```
Root cause: [what was wrong, file:line]
Fix: [what changed, file:line]
Sibling sweep: [N same-shape sites checked, N fixed / none found]
Confirmed: [evidence or test that proves the fix]
Tests: [pass/fail count, regression test location]
Regression guard: [test file:line] or [none, reason]
```
