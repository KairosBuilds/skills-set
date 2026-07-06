# Examples

## Setup Prometheus Monitoring
```bash
opencode monitoring-engineer setup prometheus --target app:8080
```

## Create Dashboard
```bash
opencode monitoring-engineer dashboard create --name api-overview --metrics latency,errors,throughput
```

## Configure Alerts
```bash
opencode monitoring-engineer alert create --name high-error-rate --condition "error_rate > 0.05"
```

## Output
Configures monitoring infrastructure with metrics collection, dashboards, alerts, and log aggregation.
