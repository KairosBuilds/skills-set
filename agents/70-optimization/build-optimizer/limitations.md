# Limitations

1. Build caching may cause stale output if cache is not invalidated
2. SWC/esbuild may not support all Babel plugins
3. Module federation adds complexity to deployment
4. Faster transpilers may produce slightly larger bundles
5. Parallel builds increase memory usage
6. CI cache size limits may restrict effectiveness
7. Some optimizations are bundler-specific and not portable
8. Migrating between bundlers requires significant refactoring
