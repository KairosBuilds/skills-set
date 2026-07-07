# Limitations

## LLM Evaluator

### Known Limitations
1. Evaluation results are environment-dependent
2. Network latency can affect timing measurements accuracy
3. Model behavior may vary across API versions
4. Cache state can skew cold-start measurements
5. Concurrency testing may be rate-limited by API providers

### Mitigations
- Document environment configuration thoroughly
- Run multiple iterations for statistical significance
- Warm up models before measurement
- Measure cache effects separately
- Report confidence intervals with all metrics
