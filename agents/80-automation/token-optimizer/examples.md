# Examples

## Example 1: Budget Warning
```
Input: "Session token usage at 82%"
Report:
- Total: 41k/50k tokens
- Input: 28k (68%)
- Output: 13k (32%)
- Top consumers: release-manager (15k), debugging (12k)
- Suggestion: compress debugging context
```

## Example 2: Optimization Opportunity
```
Input: "Review token efficiency for workflow"
Analysis:
- Average prompt: 850 tokens (target: 600)
- Average response: 1200 tokens (target: 800)
- Verbose instructions: +250 tokens extra
- Suggestion: use condensed instruction format
```

## Example 3: Cost Report
```
Input: "Weekly token usage report"
Summary:
- Total tokens: 340k (input 210k, output 130k)
- Estimated cost: $3.40
- By agent: automation (45%), release (30%), monitoring (25%)
- Trend: -12% from previous week
```
