# Examples

## Coverage Report
```
File                  % Stmts   % Branch   % Funcs   Lines
src/user/service.ts   92.5      85.7       100.0     125/135
src/user/validator.ts 45.0      30.0       50.0      9/20    ← BELOW THRESHOLD
src/payment/gateway   78.0      65.0       80.0      39/50
```

## Coverage Configuration
```json
{
  "coverageThreshold": {
    "global": { "branches": 80, "functions": 85, "lines": 85 },
    "src/user/validator.ts": { "branches": 70 }
  }
}
```
