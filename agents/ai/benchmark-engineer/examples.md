# Examples

## Benchmark Engineer

### Example 1: Accuracy Benchmark
```
Dataset: MMLU (57 subjects)
Model A: 86.4% (+/- 0.3%)
Model B: 84.2% (+/- 0.4%)
Model B is 2.2% lower (p < 0.001)
```

### Example 2: Latency Benchmark
```
Prompt length: 1500 tokens
Output length: 200 tokens

Model A: p50 1.2s, p99 2.1s
Model B: p50 0.8s, p99 1.4s
Model B is 33% faster (p50)
```

### Example 3: Multi-Metric Report
```yaml
benchmark:
  name: "model-comparison-q2"
  metrics:
    accuracy: { A: 0.92, B: 0.89 }
    latency_ms: { A: 450, B: 320 }
    cost_per_1k: { A: 0.15, B: 0.08 }
```
