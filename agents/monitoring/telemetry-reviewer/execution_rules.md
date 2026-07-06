# Execution Rules

## Instrumentation Standards
1. All HTTP/gRPC endpoints must have tracing spans
2. Database queries must be instrumented with DB span attributes
3. External service calls must create child spans
4. Background jobs must have root spans with job metadata

## Span Naming Convention
- `{service}.{operation}` format
- HTTP: `{method} {path}` (e.g., `POST /api/users`)
- DB: `{db.system}.{operation}` (e.g., `postgres.select`)
- Messaging: `{messaging.system}.{operation}` (e.g., `kafka.consume`)

## Sampling Rules
1. Production: 10% head-based sampling (adjustable)
2. Error traces: 100% sampled regardless of rate
3. Critical paths: configurable higher sampling rate
4. Development: 100% sampling

## Data Quality
1. Every span must have: trace_id, span_id, service.name, duration
2. 80%+ of endpoints must be instrumented
3. Logs must include trace_id for correlation
4. Metrics must have service and endpoint labels
