# Execution Rules

## Error Tracking Configuration
1. Install error tracking SDK in all services
2. Configure source maps/stack trace deobfuscation
3. Set environment tags (production, staging, development)
4. Configure release tracking for regression detection
5. Set user context for impacted user identification

## Alert Thresholds
1. **New Error**: Alert on first occurrence (P2)
2. **Error Spike**: >200% increase over 15min baseline (P1)
3. **Critical Error**: Payment/auth/db errors (P0)
4. **Regression**: Previously fixed error reappears (P1)

## Grouping Rules
1. Group by error fingerprint (type + stack trace)
2. Separate by environment
3. Separate by release version
4. Merge duplicates with same root cause
5. Ignore known non-actionable errors

## Incident Response
1. Acknowledge within 5min (P0), 15min (P1)
2. Investigate root cause
3. Apply fix or mitigation
4. Verify resolution
5. Document post-mortem for significant incidents
