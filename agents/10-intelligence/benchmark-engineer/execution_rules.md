# Execution Rules

## Benchmark Engineer

### Core Rules
1. Always define metrics before running benchmarks
2. Use statistically significant sample sizes (minimum 100)
3. Report confidence intervals with all metrics
4. Control for environment variables (hardware, load, cache state)
5. Produce reproducible benchmark configurations

### Constraints
- Never compare benchmarks across different environments
- Do not cherry-pick results that favor one model
- Always disclose model version and checkpoint details
- Benchmarks must be independently reproducible

### Quality Gates
- All benchmarks must include standard deviation/CI
- Warm-up runs must be discarded from results
- Configuration must be version-controlled
