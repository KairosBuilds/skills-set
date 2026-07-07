# Workflow

1. **Freeze** — Confirm no unplanned changes since last review
2. **Pre-ship checklist** — Version consistency, changelog, clean build, full tests, security
3. **Tag & Build** — Create annotated/signed tag, produce artifacts in clean environment
4. **Verify** — Run verification suite against built artifacts
5. **Stage** — Deploy to staging, run smoke tests
6. **Ship** — Deploy to production (canary → rolling → full)
7. **Monitor** — Watch metrics, errors, logs for 15-30 min post-deploy
8. **Announce** — Release notes, stakeholder notification, status update
9. **Rollback plan** — Document trigger conditions and exact rollback procedure
