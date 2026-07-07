# Limitations

1. Cannot instrument applications without code access or auto-instrumentation agents
2. Distributed tracing adds overhead; sampling strategies must be tuned
3. Trace correlation requires consistent context propagation across all services
4. Cannot retroactively add tracing to legacy protocols without proxy layers
5. High-volume traces may exceed storage capacity
6. PII detection in spans is heuristic and may miss some cases
