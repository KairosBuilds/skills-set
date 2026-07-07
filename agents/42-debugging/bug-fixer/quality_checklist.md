# Bug Fixer — Quality Checklist

## Pre-Fix
- [ ] Bug is confirmed with reproduction steps
- [ ] Root cause is identified (not just symptoms)
- [ ] All code paths affected by the fix are understood
- [ ] Existing test suite is available and runnable
- [ ] Backup of original files is created

## Fix Application
- [ ] Fix is minimal and surgical
- [ ] Code style and conventions are preserved
- [ ] Inline comments explain the change rationale
- [ ] No unrelated changes are included
- [ ] All affected files are updated consistently

## Verification
- [ ] Code compiles without errors
- [ ] Existing tests pass with the fix
- [ ] New tests cover the fixed code path
- [ ] No new warnings are introduced
- [ ] Edge cases for the fix are verified

## Output
- [ ] Diff is clean and reviewable
- [ ] Fix explanation is clear and complete
- [ ] Test results are documented
- [ ] Rollback plan is available if needed
