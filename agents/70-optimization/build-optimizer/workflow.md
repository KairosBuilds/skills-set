# Workflow

1. Profile current build times (warm and cold cache)
2. Identify slow stages (transpilation, minification, bundling)
3. Enable/build caching layer
4. Replace slow transpilers with faster alternatives (SWC, esbuild)
5. Configure parallel loaders and workers
6. Optimize loader/test patterns to exclude unnecessary files
7. Set up module federation/lazy compilation for large projects
8. Implement CI build caching (GitHub Actions cache, Docker layer caching)
9. Measure improvement and set budgets
10. Document build configuration with optimization rationale
