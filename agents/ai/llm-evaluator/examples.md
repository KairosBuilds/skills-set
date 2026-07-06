# Examples

## LLM Evaluator

### Example 1: TTFT Measurement
```
Model: gpt-4o-mini
TTFT (p50): 320ms
TTFT (p95): 580ms
Tokens/sec: 142
```

### Example 2: Concurrency Test Results
```
Concurrency 1:  100% success, p50 400ms
Concurrency 5:  100% success, p50 480ms
Concurrency 10: 100% success, p50 620ms
Concurrency 20: 98% success,  p50 890ms
```

### Example 3: Quality Comparison
```
Model A accuracy: 0.92
Model B accuracy: 0.88
Blind judge preferred: Model A (62%)
```
