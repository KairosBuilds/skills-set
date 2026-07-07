# Execution Rules

1. Profile long-running processes to catch slow leaks
2. Compare heap snapshots at different timestamps
3. Focus on retained size, not shallow size
4. Identify allocation hot spots and large object graphs
5. Reduce GC pressure by pooling reusable objects
6. Look for unintentional references preventing GC
7. Analyze object lifetimes and growth rates
8. Fix leaks one at a time and re-verify
9. Set memory budgets for critical components
10. Document memory usage patterns with heap dump evidence
