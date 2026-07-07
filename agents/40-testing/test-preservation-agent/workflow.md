# Workflow

1. Compute test baseline (file count, assertion count) for each module
2. On PR, diff test files against baseline
3. Identify deletions, skips, and coverage reductions
4. Classify each change as safe or concerning
5. Generate preservation report for the PR
6. Post findings as PR review comments
7. Track preservation metrics across releases
8. Escalate repeated violations to QA lead
