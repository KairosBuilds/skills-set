# Limitations

1. Cannot optimize client-side network conditions (last mile)
2. CDN configuration depends on provider capabilities
3. HTTP/2 requires TLS (SSL termination overhead)
4. gRPC is not suitable for browser clients natively
5. Some corporate networks block HTTP/2 or WebSockets
6. Protocol optimization may not help with small payloads
7. Cannot control third-party API network performance
8. WebSocket optimizations depend on client implementation
