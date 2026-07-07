# Execution Rules

1. Do not touch code until root cause can be stated in one sentence with file:line evidence
2. Same symptom after a fix is a hard stop — re-read execution path from scratch
3. After 3 failed hypotheses, stop and produce handoff report
4. Verify all claims with commands — never use memory for versions, locations, or names
5. For regressions ("used to work"), use bisect with a non-interactive pass/fail test
6. After fixing a root-cause pattern, run scope blast mode to find sibling instances
7. Every recurring bug fix must include a regression test
