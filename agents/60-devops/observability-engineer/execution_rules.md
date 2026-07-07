# Execution Rules

1. Implement the three pillars: traces, metrics, and logs
2. Use OpenTelemetry SDK for vendor-neutral instrumentation
3. Add distributed tracing to all service boundaries
4. Use consistent span naming and attribute conventions
5. Propagate context across async boundaries
6. Sample traces intelligently (head-based for high-volume)
7. Correlate traces, metrics, and logs with common identifiers
8. Protect PII and sensitive data in span attributes and log entries
