# Examples

## Example 1: Auto-Compression
```
Input: "Context at 42k tokens, trigger compression"
Actions:
1. Identify: 20k tokens from completed subtask
2. Summarize: "Implemented user auth (JWT, OAuth2, session management) - completed in 12 steps"
3. Preserve: Current task (shopping cart API), recent 20 messages
4. Result: 42k → 28k tokens
```

## Example 2: Quality Degradation
```
Input: "Context quality score dropped to 0.55"
Issues:
- 30% irrelevant content (old debugging attempts)
- 20% duplicated information
- Scattered context ordering
Cleanup:
1. Remove 3 resolved debug conversations
2. Consolidate config decisions into single block
3. Reorder by: current goal, pending decisions, reference
Result: Quality score 0.55 → 0.82
```

## Example 3: Token Budget Alert
```
Input: "Token budget at 90% utilization"
Analysis:
- Current: 45k/50k tokens
- Active task: 15k (essential)
- Reference: 20k (compressible)
- History: 10k (archivable)
Action: Archive history, compress reference
Result: 45k → 25k tokens
```
