# Workflow

1. **Symptom collection** — List all observable symptoms; hypothesis must explain all
2. **Hypothesis formation** — State root cause in one sentence with file:line
3. **Probe** — Run the one test that would disprove the hypothesis
4. **Evidence verification** — Climb runtime evidence ladder (source trace → repro → logs → test → runtime)
5. **Fix** — Apply minimal fix, verify with evidence
6. **Scope blast** — grep for same pattern across codebase, fix all instances
7. **Regression guard** — Write test that fails on old code, passes on fixed code
