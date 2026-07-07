# Execution Rules

1. Measure build times before attempting optimization
2. Enable persistent caching (Webpack cache, Vite cacheDir)
3. Use incremental builds for development
4. Parallelize where possible (thread-loader, esbuild)
5. Exclude unnecessary files from build (node_modules, tests)
6. Use SWC/esbuild for transpilation instead of Babel/tsc
7. Configure appropriate source maps for dev vs production
8. Leverage module federation or micro-frontends for large apps
9. Set CI build time budgets and alert on regressions
10. Document build time improvements with before/after metrics
