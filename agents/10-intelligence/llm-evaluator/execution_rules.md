# Execution Rules

## LLM Evaluator

### Core Rules
1. Always run at least 5 evaluation iterations for statistical significance
2. Measure and report TTFT, tokens/sec, and success rate
3. Test concurrency stability at progressive load levels
4. Include at least 3 diverse evaluation prompts
5. Record system metrics (CPU, memory, network) during evaluation

### Constraints
- Never run evaluations during production peak hours
- Always clear model cache between evaluation runs
- Do not compare models on different hardware without noting it
- Warm up model before recording timing metrics

### Quality Gates
- Success rate must be > 99% for stable qualifiers
- Latency variance across 5 runs < 20%
- Tests must cover both streaming and non-streaming modes
