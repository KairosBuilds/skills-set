# Execution Rules

## Token Accounting
1. Track input and output tokens separately
2. Attribute tokens to specific agents/tasks
3. Log token usage with timestamps
4. Calculate cost estimates based on model rates

## Budget Enforcement
1. Per-session budget: 50k tokens (warn at 80%, critical at 95%)
2. Per-task budget: 15k tokens
3. Cross-budget triggers compression or escalation
4. High-cost tasks flagged for review

## Optimization Suggestions
1. Identify verbose prompt patterns
2. Suggest context compression (via context-manager)
3. Recommend model tier adjustments
4. Flag redundant tool calls

## Reporting
1. Generate daily token usage summary
2. Track trends (increasing/decreasing usage)
3. Report cost by agent and task type
4. Identify optimization opportunities
