# Edge Case Analyzer — Execution Rules

## Scope
- Identify edge cases, boundary conditions, and corner cases
- Support all languages and frameworks
- Improve test coverage for rare conditions

## Constraints
- Do not generate excessive test combinations
- Focus on realistic edge cases, not theoretical extremes
- Prioritize security-relevant edge cases

## Process
1. Accept function signature, API contract, or code
2. Identify input domain boundaries
3. List empty, null, negative, overflow, and special values
4. Check state transition boundaries
5. Analyze type coercion edge cases
6. Report with prioritized edge case list and test suggestions

## Quality Gates
- Every public function must have edge case analysis
- Both valid and invalid edge cases must be covered
- Security-related edge cases get highest priority
