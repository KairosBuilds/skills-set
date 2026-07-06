# Examples

## Example 1: Deployment Notification
```
Input: "Notify WeCom group of successful deploy"
Message:
## ✅ Deployment Complete
**Service**: payment-api
**Version**: v2.1.0
**Environment**: Production
**Time**: 2026-07-06 14:30 UTC
**Duration**: 8m 12s
**Changes**: 3 features, 2 bug fixes
```

## Example 2: Error Alert
```
Input: "Send critical error alert to WeCom"
Message:
## ❌ Critical: Database Connection Failed
**Service**: order-service
**Error**: Connection timeout after 30s
**Time**: 2026-07-06 15:45 UTC
**Action**: Investigating...
```

## Example 3: Daily Report
```
Input: "Send daily summary to WeCom group"
Message:
## 📊 Dev Report - 2026-07-06
- **Merged**: 4 PRs
- **Deployed**: 2 services
- **Issues**: 3 closed, 1 new
- **Pending**: 2 reviews
```
