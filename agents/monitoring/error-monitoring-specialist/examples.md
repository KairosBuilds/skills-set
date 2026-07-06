# Examples

## Example 1: Sentry Configuration
```
Input: "Configure Sentry for Node.js services"
Actions:
1. Install @sentry/node in each service
2. Initialize with DSN per environment
3. Configure source maps upload
4. Set release tracking via git SHA
5. Configure error grouping by fingerprint
6. Set up Slack alerts for new errors
7. Create dashboard for top errors by volume
```

## Example 2: Spike Investigation
```
Input: "Error rate increased 500% on checkout-service"
Actions:
1. Open Sentry dashboard for checkout-service
2. Filter by last 15 minutes
3. Identify: Database connection timeout errors
4. Check: recent deployment (new connection pool settings)
5. Rollback connection pool changes
6. Verify error rate returns to baseline
```

## Example 3: Regression Detection
```
Input: "Previously fixed SQL injection error reappeared"
Actions:
1. Identify error fingerprint
2. Check resolved issues list
3. Find original fix was in v1.2.0
4. Current version: v1.4.0 (regression)
5. Re-open original ticket
6. Apply fix again with regression test
```
