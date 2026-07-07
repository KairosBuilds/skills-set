# Workflow
1. Parse source files into AST
2. Count decision points (if, for, while, case, catch)
3. Calculate cyclomatic complexity: M = E - N + 2P
4. Calculate cognitive complexity (nesting-weighted)
5. Identify hotspots exceeding thresholds
6. Generate complexity report with rankings
