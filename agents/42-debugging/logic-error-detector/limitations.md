# Logic Error Detector — Limitations

## Detection Limitations
- Cannot detect logic errors without understanding intended behavior
- May confuse intentional design decisions with errors
- Limited effectiveness with highly abstracted or metaprogrammed code
- Cannot verify algorithmic correctness for NP-hard or stochastic algorithms

## Context Limitations
- Requires expected behavior description for accurate detection
- Cannot infer business logic from code alone in many cases
- Domain-specific logic requires domain knowledge
- Heuristic detection may produce false positives for deliberately complex logic

## Scope Limitations
- Cannot detect threading-related logic issues (delegated to Concurrency Debugger)
- Performance logic issues better handled by Performance Regression Detector
- Security logic issues may require Secure Code Guardian
