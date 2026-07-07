# Workflow

1. Record performance profile in Chrome DevTools
2. Identify long frames and jank sources
3. Profile React component renders (React Profiler)
4. Identify wasted renders (components that render without prop changes)
5. Check for layout thrashing in requestAnimationFrame loops
6. Analyze WebGL draw calls and shader complexity
7. Implement optimizations (memo, virtualization, lazy loading)
8. Re-profile and compare frame times
9. Verify on target device (mobile/low-end hardware)
10. Document rendering budget and key metrics
