# Examples

## Example 1: PR Creation
```
Input: "Create PR for feature/new-login"
Actions:
1. Check branch exists and is ahead of main
2. Generate PR title: "feat: add OAuth2 login support"
3. Generate description with changes list
4. Link issue #142
5. Request review from @team-lead, @security
6. Enable auto-merge if all checks pass
```

## Example 2: Issue Triage
```
Input: "Triage new issues for sprint planning"
Actions:
1. List all unassigned issues
2. Categorize by label (bug, feature, enhancement)
3. Assign priority based on labels
4. Assign to sprint backlog
5. Notify team of high-priority items
```

## Example 3: Workflow Debug
```
Input: "CI workflow failing on main branch"
Actions:
1. Check latest workflow run
2. Identify failing step (lint)
3. Review error output
4. Fix lint issues in PR
5. Re-run workflow
6. Merge fix to main
```
