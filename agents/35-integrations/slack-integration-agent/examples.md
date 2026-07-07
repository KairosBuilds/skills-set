# Examples

## Example 1: Release Notification
```
Input: "Notify team of successful deployment"
Message:
🚀 v2.1.0 Deployed to Production
• Features: CSV export, dark mode
• Fixes: login timeout, date formatting
• Duration: 12min (3min faster than previous)
• Rollback: git revert v2.1.0
```

## Example 2: Alert
```
Input: "Send build failure alert"
Message:
❌ Build Failed: main branch
• Commit: a1b2c3d - "feat: add payment"
• Error: TypeScript compilation error (5 errors)
• Author: @dev
• Fix: check type definitions
```

## Example 3: Daily Summary
```
Input: "Send end-of-day summary"
Message:
📊 Daily Summary - 2026-07-06
• PRs merged: 3
• Issues closed: 5
• Deployments: 2 (staging), 1 (production)
• Pending reviews: 1
• Blockers: payment API integration
```
