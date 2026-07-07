# Examples

## Define SLOs
```bash
opencode sre-engineer slo define --service api-gateway --latency-p99 200ms --availability 99.95
```

## Setup Error Budget Alerts
```bash
opencode sre-engineer alert setup --service api-gateway --burn-rate 2 --window 1h
```

## Create SLO Dashboard
```bash
opencode sre-engineer dashboard create --service api-gateway
```

## Output
Configures SLO tracking, error budget monitoring, and alerting for service reliability management.
