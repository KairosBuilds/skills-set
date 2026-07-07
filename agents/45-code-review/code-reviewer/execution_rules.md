# Execution Rules

## Scope
- Analyze all source files in the review scope
- Do not modify files during review
- Report findings with severity classification

## Rules
1. Always read the full file before commenting
2. Classify each finding by severity (critical/high/medium/low/info)
3. Provide actionable remediation suggestions
4. Do not report false positives - verify before flagging
5. Respect .gitignore and configured exclude patterns
6. Check for test coverage alongside production code
7. Report N+1 queries and performance antipatterns
8. Flag hardcoded secrets and credentials immediately
9. Consider the broader architectural context
10. Generate structured markdown reports

## Output Format
Every finding must include: file path, line number, severity, description, and suggested fix.
