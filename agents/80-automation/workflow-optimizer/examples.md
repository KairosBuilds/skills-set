# Examples

## Example 1: CI Pipeline Optimization
```
Input: "CI pipeline takes 25 minutes, optimize"
Analysis:
- Test stage: 15min (sequential, 400 tests)
- Build stage: 8min (caching disabled)
- Lint stage: 2min
Recommendations:
1. Split tests across 4 parallel runners (15min → 5min)
2. Enable build caching (8min → 3min)
3. Run lint in parallel with build (saves 2min)
Projected: 25min → 10min
```

## Example 2: Context Health Warning
```
Input: "Agent context exceeding optimal range"
Analysis:
- Current context: 85k tokens
- Optimal range: 30-50k tokens
- Action: Trigger context compression
- Recommendation: Archive completed tasks
```

## Example 3: Test Bottleneck
```
Input: "Integration tests too slow"
Analysis:
- Sequential execution: 30min
- No database caching: each test resets DB
- Recommendations:
  1. Parallelize test files (30min → 8min)
  2. Use DB snapshot for test setup
  3. Run critical tests first
```
