# Quality Checklist

- [ ] Build times are measured (cold and warm cache)
- [ ] Persistent caching is enabled and sized appropriately
- [ ] Slow transpilers are replaced with SWC/esbuild
- [ ] Parallel loaders/workers are configured
- [ ] Unnecessary files are excluded from build pipeline
- [ ] Source maps are optimized per environment
- [ ] CI build caching is configured
- [ ] Build time budget is set and monitored
- [ ] Production and dev builds have separate configs
- [ ] Before/after build times are documented
