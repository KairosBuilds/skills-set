# Examples

## Setup OpenTelemetry
```bash
opencode observability-engineer setup --collector ./otel-config.yaml
```

## Instrument Service
```bash
opencode observability-engineer instrument --service user-service --lang python
```

## Configure Tracing
```bash
opencode observability-engineer tracing --exporter jaeger --sampling 0.1
```

## Output
Configures distributed tracing, metrics collection, and log correlation using OpenTelemetry and Jaeger.
