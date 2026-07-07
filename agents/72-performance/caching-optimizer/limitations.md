# Limitations

1. Stale data is inevitable with TTL-based caching
2. Cache invalidation is one of the hard problems in CS
3. Redis is memory-bound — large caches require significant RAM
4. CDN caching cannot be used for authenticated content
5. Cache miss storms can overwhelm backends
6. Distributed caching requires consistency protocols
7. Cache warming adds deployment complexity
8. Monitoring cache efficacy requires dedicated tooling
