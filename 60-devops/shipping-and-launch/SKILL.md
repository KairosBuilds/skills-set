---
name: shipping-and-launch
description: Production release workflow covering version bumping, changelog generation, tagging, building, publishing, rollout verification, and rollback planning. Use when preparing a release, shipping to production, or launching a new version. Not for daily development or feature work.
license: MIT
compatibility: opencode
metadata:
  author: "Prateek"
  version: "1.0.0"
  domain: devops
  triggers: release, ship, deploy, publish, launch, version bump, tag, changelog, go live
  role: specialist
  scope: deployment
  output-format: workflow
  related-skills: definition-of-done, git-release, incremental-implementation, code-reviewer
---

# Shipping and Launch

Production release workflow. Every release carries risk; this skill minimizes it through verification, rollout planning, and rollback readiness.

## Pre-Ship Checklist

Before any release, verify these gates:

### Version Consistency
- Version bumped in all manifests (package.json, Cargo.toml, etc.) — same value everywhere
- Changelog updated with entries for this release
- Tag matches the version (vX.Y.Z format)

### Build Artifacts
- Clean build passes (from scratch, not incremental)
- Generated artifacts are deterministic or reproducible
- Artifact size is expected (no accidental bloat)
- Checksums/signatures generated where applicable

### Test Gates
- Full test suite passes
- Integration/E2E tests pass against build artifacts
- Performance benchmarks show no regression

### Safety Checks
- Rollback plan exists and is tested
- Feature flags are in correct state (enabled/disabled as intended)
- Database migrations are reversible
- No secrets hardcoded in build artifacts

## Ship Workflow

1. **Freeze** — Confirm no unplanned changes have been merged since last review
2. **Tag** — Create signed/annotated tag matching version
3. **Build** — Produce release artifacts in clean environment
4. **Verify** — Run verification suite against built artifacts
5. **Stage** — Deploy to staging/pre-prod environment
6. **Smoke test** — Run critical path checks against staged deployment
7. **Ship** — Deploy to production (canary → rolling → full)
8. **Monitor** — Watch metrics, errors, and logs for 15-30 minutes post-deploy
9. **Announce** — Update status, notify stakeholders, publish release notes

## Rollback Plan

Every release must have a documented rollback plan:

```
Rollback trigger: [which signals would trigger rollback]
Rollback method: [git revert / database restore / feature flag / artifact redeploy]
Rollback duration: [estimated time to rollback]
Verification: [how to confirm rollback succeeded]
```

## Canary/Progressive Delivery

For high-risk releases:

1. **1% canary** — Route 1% of traffic to new version. Monitor for 10+ minutes.
2. **10%** — Increase to 10%. Monitor errors, latency, business metrics.
3. **50%** — Half of traffic. Confirm no degradation.
4. **100%** — Full rollout. Continue monitoring.

## Release Notes Template

```
## [vX.Y.Z] - YYYY-MM-DD

### Added
- [new feature 1]
- [new feature 2]

### Changed
- [behavior change 1]

### Fixed
- [bug fix 1]
- [bug fix 2]

### Security
- [security fix 1]
```

## Output

```
Release: vX.Y.Z
Status: [shipped / rolled back / in progress]
Artifacts: [links or paths]
Verification: [test results, smoke test status]
Rollback: [plan name, tested yes/no]
Monitors: [dashboard links, alert names]
```
