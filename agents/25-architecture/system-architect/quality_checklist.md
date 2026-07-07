# System Architect Quality Checklist

## Pre-Delivery Validation

### Requirements Coverage
- [ ] All scalability requirements addressed
- [ ] Reliability targets defined (SLA/SLO)
- [ ] Performance characteristics estimated
- [ ] Operational requirements covered

### Design Quality
- [ ] System boundaries clearly defined
- [ ] Component decomposition is logical
- [ ] Communication patterns are well-defined
- [ ] Failure modes analyzed for each component

### Scalability
- [ ] Scaling model defined (horizontal/vertical)
- [ ] Load distribution strategy documented
- [ ] Data partitioning strategy defined
- [ ] Bottlenecks identified and mitigation planned
- [ ] Capacity growth projections included

### Reliability
- [ ] Redundancy and failover mechanisms designed
- [ ] Circuit breaker and retry policies defined
- [ ] Disaster recovery plan included
- [ ] RPO and RTO targets stated

### Operations
- [ ] Observability strategy defined (metrics, logs, traces)
- [ ] Deployment strategy documented
- [ ] Incident response plan included
- [ ] Runbooks referenced or outlined

## Scoring Rubric

| Criterion | Weight | Pass Threshold |
|-----------|--------|---------------|
| Requirements Coverage | 15% | 100% |
| Design Quality | 20% | >= 90% |
| Scalability | 25% | >= 90% |
| Reliability | 25% | >= 90% |
| Operations | 15% | >= 85% |
| **Overall** | **100%** | **>= 95%** |
