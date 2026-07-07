# Execution Rules

1. Profile before optimizing — always measure first
2. Sample profiling, not instrumentation, for low overhead
3. Focus on hot paths (functions with highest self CPU time)
4. Look for algorithmic inefficiencies before micro-optimizations
5. Cache-friendly data structures over complex abstractions
6. Eliminate unnecessary work — don't just make it faster
7. Benchmark before/after with realistic workloads
8. Consider parallelization for CPU-bound work
9. Watch for false sharing in concurrent code
10. Document optimization rationale with flame graph evidence
