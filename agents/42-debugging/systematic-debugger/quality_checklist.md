# Quality Checklist

- [ ] Root cause stated as one sentence with file:line before any code change
- [ ] Hypothesis explains all observed symptoms
- [ ] Each claim verified with command output (not memory)
- [ ] For regressions: bisect with non-interactive test
- [ ] Scope blast completed after fix
- [ ] Regression guard test exists for recurring bugs
- [ ] After 3 failed hypotheses: handoff produced
- [ ] Fix touches minimal files (flag if >5)
