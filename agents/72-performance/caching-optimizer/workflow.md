# Workflow

1. Analyze current cache setup and hit rates
2. Identify uncached hot paths and high-latency queries
3. Design multi-layer caching strategy (browser → CDN → app → DB)
4. Configure HTTP cache headers (Cache-Control, ETag)
5. Set up Redis/Memcached with appropriate TTL and eviction policy
6. Implement cache-aside or read-through pattern in application
7. Set up CDN edge caching for static and semi-static content
8. Implement cache invalidation on data mutations
9. Monitor cache metrics (hit rate, latency, memory usage)
10. Tune TTLs and eviction policies based on usage patterns
