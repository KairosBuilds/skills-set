# Execution Rules

1. Measure network performance with realistic connection profiles
2. Enable HTTP/2 multiplexing where supported
3. Configure CDN for edge caching and origin shielding
4. Use connection pooling for database and API connections
5. Compress responses (gzip, brotli) — always
6. Reduce payload sizes with field selection and pagination
7. Implement keep-alive and reuse connections
8. Use gRPC for internal service-to-service communication
9. Optimize WebSocket message framing and batching
10. Monitor DNS resolution times and TTFB
