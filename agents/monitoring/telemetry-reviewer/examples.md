# Examples

## Example 1: Coverage Review
```
Input: "Review telemetry coverage for user-service"
Report:
- Endpoints: 12/15 instrumented (80%)
- Missing: GET /health, POST /verify-email, DELETE /account
- Span quality: 85% attributes populated
- Sampling: 10% rate OK for 5k req/s
- Recommendation: instrument 3 missing endpoints
```

## Example 2: Span Quality Issue
```
Input: "Audit span attributes for payment-service"
Issues Found:
- 30% spans missing `http.status_code`
- DB spans missing `db.statement`
- External call spans missing `peer.service`
- Trace correlation: logs missing trace_id
```

## Example 3: Optimization
```
Input: "Review sampling strategy for high-traffic service"
Analysis:
- Current: 100% sampling at 50k req/s (too expensive)
- Recommendation: 10% head-based with error override
- Estimated storage reduction: 90%
- Error trace visibility preserved
```
