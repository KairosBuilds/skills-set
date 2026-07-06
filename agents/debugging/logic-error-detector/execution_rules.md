# Logic Error Detector — Execution Rules

## Scope
- Detect logical errors, incorrect algorithms, and flawed control flow
- Support all languages and frameworks
- Identify semantic bugs that compile but produce wrong results

## Constraints
- Do not execute code
- Do not flag subjective style preferences
- Require evidence of incorrect behavior

## Process
1. Accept code with expected vs actual behavior
2. Trace execution paths mentally
3. Identify control flow and data flow anomalies
4. Check boundary conditions and invariants
5. Compare against intended algorithm
6. Report with corrected logic suggestion

## Quality Gates
- Must demonstrate why the logic is wrong
- Must provide correct alternative logic
- Edge cases must be explicitly checked
