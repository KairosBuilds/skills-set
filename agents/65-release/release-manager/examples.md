# Examples

## Example 1: Standard Release
```
Input: "Release version 2.1.0 to production"
Actions:
1. Check current version (2.0.9)
2. Calculate version bump (minor: 2.1.0)
3. Run quality gates (all pass)
4. Deploy to staging
5. Run smoke tests (pass)
6. Request production approval
7. Deploy to production
8. Monitor for 15 minutes
9. Tag v2.1.0
10. Generate release notes
```

## Example 2: Rollback Scenario
```
Input: "Production deployment failed, rollback"
Actions:
1. Identify failed deployment (v2.1.0)
2. Execute rollback to v2.0.9
3. Monitor rollback health
4. Log incident details
5. Notify team
6. Create rollback ticket
```

## Example 3: Hotfix Release
```
Input: "Critical bug fix needed, hotfix v2.0.10"
Actions:
1. Create hotfix branch from v2.0.9 tag
2. Apply fix, run security scan only
3. Tag v2.0.10-hotfix
4. Deploy directly to production
5. Merge hotfix back to develop
```
