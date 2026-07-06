# Examples

## Example 1: Service Observability Setup
```
Input: "Set up observability for payment-service"
Actions:
1. Deploy Prometheus for metrics collection
2. Configure Loki for log aggregation
3. Set up Tempo for distributed tracing
4. Instrument service with RED metrics
5. Define SLO: 99.95% uptime, p95 latency <500ms
6. Create Grafana dashboard (4 panels)
7. Configure alerts: error rate >1%, p99 >2s
```

## Example 2: SLO Definition
```
Input: "Define SLOs for API gateway"
SLIs:
- Request success rate (>=99.9%)
- Response time p95 (<300ms)
- Availability (>=99.99%)
SLO: 
- 99.9% requests succeed within 300ms over 30 days
Error budget: 0.1% = 43m 12s downtime/month
Burn rate: 2x for 6h, 10x for 30min
```

## Example 3: Incident Response
```
Input: "PagerDuty alert - high error rate on orders-service"
Actions:
1. Check Grafana dashboard
2. Determine scope (all endpoints or specific)
3. Check recent deployments
4. Trace sample error to identify root cause
5. Escalate if needed
```
