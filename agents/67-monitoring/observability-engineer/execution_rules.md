# Execution Rules

## Metrics Standards
1. RED metrics for every service: Rate, Errors, Duration
2. USE metrics for infrastructure: Utilization, Saturation, Errors
3. Standard labels: service, environment, endpoint, method, status
4. Metrics must have consistent naming: `{namespace}_{name}_{unit}`

## SLO Definitions
1. Define SLIs that reflect user-facing reliability
2. SLO target: 99.9% default, adjustable per service tier
3. Error budget: 100% - SLO target (monthly window)
4. Burn rate alerts for faster incident detection

## Alerting Rules
1. P0: Service down or data loss — immediate (5min response)
2. P1: Degraded performance — urgent (15min response)
3. P2: Warning signs — next business day
4. P3: Informational — no action required
5. P4: Long-term trends — tracked in backlog

## Dashboard Design
1. Every service needs: RED metrics, top errors, latency heatmap
2. System dashboards: CPU, memory, disk, network
3. Business dashboards: user signups, orders, revenue
4. All dashboards must include time range selector and refresh control
