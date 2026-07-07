# Quality Checklist

## Pre-Fix
- [ ] Issue clearly identified and isolated
- [ ] Edit loop count checked
- [ ] Fix scope understood (single vs multi-file)
- [ ] Rollback plan ready

## During Fix
- [ ] Fix is minimal (no unrelated changes)
- [ ] No silent behavior changes
- [ ] Merge conflict resolution preserves both intents
- [ ] Edit loop break provides new approach

## Post-Fix
- [ ] Verification passes (build, lint, typecheck)
- [ ] Tests pass (related tests)
- [ ] Rollback available if needed
- [ ] Fix logged with outcome
- [ ] Success rate metrics updated
