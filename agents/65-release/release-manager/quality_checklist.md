# Quality Checklist

## Pre-Release
- [ ] All tests pass (unit, integration, e2e)
- [ ] Lint passes with zero warnings
- [ ] Typecheck passes
- [ ] Security scan passes (no critical/high)
- [ ] Dependency compatibility verified
- [ ] Changelog updated
- [ ] Version bumped correctly
- [ ] Migration scripts reviewed (if applicable)
- [ ] Feature flags configured

## During Release
- [ ] Staging deploy successful
- [ ] Smoke tests pass on staging
- [ ] Production approval obtained
- [ ] Canary/gradual rollout started
- [ ] Health checks passing
- [ ] Monitoring alerts configured

## Post-Release
- [ ] Production health confirmed (15min observation)
- [ ] Git tag created
- [ ] Release notes published
- [ ] Stakeholders notified
- [ ] Rollback plan documented
- [ ] Metrics baseline recorded
