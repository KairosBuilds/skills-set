# Runtime Error Specialist — Quality Checklist

## Pre-Analysis
- [ ] Error type, message, and stack trace are collected
- [ ] Input data that triggered the error is available
- [ ] Code context around the error location is accessible

## Analysis
- [ ] Error type is correctly classified
- [ ] Error origin is traced to exact location
- [ ] Input characteristics causing the error are identified
- [ ] Missing validation or check is pinpointed
- [ ] All paths to the error location are considered

## Fix Strategy
- [ ] Defensive programming pattern is appropriate
- [ ] Null/undefined checks are comprehensive
- [ ] Type checks are sufficient
- [ ] Boundary checks are in place
- [ ] Error handling is graceful (no silent failures)

## Output
- [ ] Root cause is clearly explained
- [ ] Triggering input pattern is documented
- [ ] Fix code is provided with defensive patterns
- [ ] Prevention strategy for similar errors is included
