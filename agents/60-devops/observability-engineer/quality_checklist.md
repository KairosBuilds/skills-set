# Quality Checklist

- [ ] OpenTelemetry SDK is configured for each service
- [ ] Distributed tracing covers all service boundaries
- [ ] Span names follow a consistent naming convention
- [ ] Trace context is propagated across async boundaries
- [ ] RED metrics are collected for all services
- [ ] Log entries include trace IDs for correlation
- [ ] Sampling strategy is configured appropriately
- [ ] Collector is configured with proper exporters
- [ ] Dashboards show traces, metrics, and logs in context
- [ ] PII is not exposed in span attributes or logs
