# Performance Regression Detector — Dependencies

## Internal Dependencies
- **Bug Finder:** Locates code changes causing regressions
- **Memory Leak Detector:** Identifies memory-related performance issues

## Tool Dependencies
- Lighthouse CLI
- CI benchmark infrastructure
- Profiling tools (flamegraph, perf)
- Bundle analysis tools (webpack-bundle-analyzer)

## Runtime Dependencies
- Baseline performance data
- Current performance data
- Build artifacts for comparison
- Network access for Lighthouse runs
