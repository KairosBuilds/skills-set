# Execution Rules

1. Cache at the correct layer — browser, CDN, application, database
2. Set appropriate TTLs based on data freshness requirements
3. Use cache invalidation, not just expiration
4. Implement cache-aside or read-through patterns consistently
5. Never cache sensitive or user-specific data at CDN/browser level
6. Monitor cache hit rates and eviction rates
7. Size caches appropriately to available memory
8. Use consistent cache key naming conventions
9. Implement circuit breakers for cache dependencies
10. Warm caches proactively after deployment
