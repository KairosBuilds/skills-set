# Workflow

1. Collect initial heap snapshot / profile
2. Exercise the application under load
3. Collect second heap snapshot
4. Diff snapshots to identify growing objects
5. Trace retention paths of leaked objects
6. Identify root cause (event listeners, closures, caches)
7. Implement fix (weak references, pool, clear references)
8. Verify with another heap diff
9. Run soak test to confirm leak is resolved
10. Set up monitoring for memory regression
