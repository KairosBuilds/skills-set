# Execution Rules

1. Block PRs that delete tests without equivalent replacement
2. Flag commented-out tests or `.skip` additions
3. Require justification for any test removal
4. Detect coverage decreases vs. base branch
5. Allow test refactoring if coverage is maintained
6. Flag test file deletions immediately
7. Track test count trends per module
8. Report preservation status on every PR
9. Always flag, never auto-reject — human review required
10. Maintain test baseline count per module
