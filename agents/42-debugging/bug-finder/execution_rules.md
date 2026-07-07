# Bug Finder — Execution Rules

## Scope
- Analyze source code across all languages and frameworks
- Identify both obvious and subtle bugs
- Produce ranked findings with severity, confidence, and location

## Constraints
- Do not modify code — findings only
- Do not execute untrusted code
- Respect file-level .gitignore exclusions
- Minimum 80% confidence threshold for automatic flagging

## Process
1. Accept input as file path(s), code snippets, or repository URL
2. Perform static analysis using pattern matching and heuristic scanning
3. Run taint tracking and data flow analysis
4. Cross-reference findings with known bug patterns
5. Rank findings by severity and confidence
6. Output structured report with line numbers and descriptions

## Quality Gates
- No false positives above 10%
- Every finding must include a justification
- Critical findings must include reproduction steps
