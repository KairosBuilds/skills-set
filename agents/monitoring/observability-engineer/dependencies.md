# Dependencies

## Internal Agents
- **logging-specialist**: Structured log pipeline
- **telemetry-reviewer**: Trace instrumentation quality
- **error-monitoring-specialist**: Error tracking integration

## External Tools
- **Prometheus**: Metrics collection and alerting
- **Grafana**: Dashboards and visualization
- **Loki**: Log aggregation
- **Tempo/Jaeger**: Distributed tracing
- **Alertmanager**: Alert routing and deduplication

## Runtime Requirements
- Kubernetes cluster or Docker hosts for stack deployment
- Persistent storage for metrics and logs
- Network access to all instrumented services
