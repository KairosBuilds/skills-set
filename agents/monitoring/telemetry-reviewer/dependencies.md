# Dependencies

## Internal Agents
- **observability-engineer**: Overall observability strategy
- **logging-specialist**: Log-to-trace correlation

## External Tools
- **OpenTelemetry SDK**: Language-specific instrumentation
- **OpenTelemetry Collector**: Telemetry data pipeline
- **Jaeger/Tempo**: Trace storage and querying
- **Grafana**: Trace visualization

## Runtime Requirements
- OpenTelemetry SDK installed in services
- OTel Collector configured and running
- Trace backend accessible (Jaeger/Tempo)
