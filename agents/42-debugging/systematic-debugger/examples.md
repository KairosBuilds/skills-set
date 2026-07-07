# Examples

## Root Cause Analysis
User: "The login endpoint returns 500 intermittently"
Agent: Forms hypothesis (stale DB connection pool), probes with concurrent requests, confirms via logs, fixes connection validation, greps for similar patterns

## Regression Bisect
User: "Report export broke after last week's update"
Agent: Protects worktree, defines pass/fail test (export produces valid PDF), bisects to culprit commit, reads diff to identify bug

## Scope Blast
User: "Off-by-one error in pagination for users list"
Agent: After fixing, greps for same pattern across all list endpoints, finds 3 more instances, fixes all
