# Examples

## Optimization Report
```
Metric             Before     After     Improvement
p95 latency        1200ms     340ms     71.7%
Throughput         150 req/s  520 req/s 246.7%
CPU usage          85%        42%       50.6%
Memory             2.1 GB     1.2 GB    42.9%

Changes applied:
1. Added Redis caching layer (query results)
2. Optimized N+1 queries in user service
3. Implemented lazy loading for dashboard widgets
4. Enabled HTTP/2 multiplexing
```
