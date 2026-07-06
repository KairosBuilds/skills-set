# Performance Regression Detector — Limitations

## Data Limitations
- Requires reliable baseline measurements for comparison
- Performance metrics are inherently noisy and require statistical analysis
- Environmental differences (hardware, load, network) affect results
- Cold start vs warm performance can vary significantly

## Detection Limitations
- Cannot detect regressions without both baseline and current data
- Small regressions (<5%) may not be statistically significant
- Micro-benchmarks may not reflect real-world performance
- Intermittent performance issues (GC pauses, JIT warmup) may cause false positives

## Tool Limitations
- Lighthouse requires a browser rendering environment
- CI benchmarks need consistent hardware allocation
- Bundle analysis needs build artifacts from both versions
- Profiling tools may affect the metrics they measure

## Scope Limitations
- Database query performance is better handled by database-optimizer
- Network latency regressions require network-level tools
- User-perceived performance has subjective components
