# Workflow

1. Attach CPU profiler (pprof, perf, Instruments)
2. Generate CPU flame graph
3. Identify hotspots — functions with >5% CPU time
4. Analyze algorithmic complexity of hot paths
5. Check for unnecessary allocations, serialization, copies
6. Implement optimization (algorithm change, caching, inlining)
7. Re-profile and compare flame graphs
8. Benchmark throughput or latency improvement
9. Verify no regression in other metrics
10. Document with before/after flame graph diff
