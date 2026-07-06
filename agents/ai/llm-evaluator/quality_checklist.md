# Quality Checklist

## LLM Evaluator

### Setup
- [ ] Evaluation parameters defined
- [ ] Test prompts selected (min 3 diverse)
- [ ] Environment configuration documented
- [ ] Warm-up runs completed (min 2)

### Execution
- [ ] Min 5 evaluation iterations per configuration
- [ ] Concurrency tested at multiple levels
- [ ] Both streaming and non-streaming tested
- [ ] System metrics captured (CPU, memory, network)

### Reporting
- [ ] TTFT reported (p50, p90, p99)
- [ ] Tokens/sec reported
- [ ] Success rate reported with sample size
- [ ] Confidence intervals included
- [ ] Environment configuration documented
