# Examples

## PR Review Comment
```
⚠️ Test Preservation Alert — src/user/service.test.ts

- 3 tests removed (line 45-62): `should validate email`, `should reject invalid email`, `should handle empty email`
- 1 test skipped (line 88): `should update user profile`

These removals reduce module coverage from 92% to 87%.
Justification required before merging.

Tests at risk of deletion:
  - src/user/validator.test.ts → coverage drops below threshold
```

## Preservation Report
```
Module: src/payment/
Baseline tests: 45
Current tests: 42 (-3)
Coverage change: 88% → 85% (-3%)
Status: ❌ Needs review
```
