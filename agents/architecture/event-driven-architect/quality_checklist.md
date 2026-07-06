# Event-Driven Architect Quality Checklist

## Pre-Delivery Validation

### Event Discovery
- [ ] All business events identified and documented
- [ ] Event producers and consumers mapped
- [ ] Event criticality assessed

### Broker Selection
- [ ] Requirements evaluated (throughput, latency, retention, routing)
- [ ] Multiple brokers compared
- [ ] Selection rationale documented in ADR

### Schema Design
- [ ] Event schemas defined for all events
- [ ] Schema format chosen with rationale
- [ ] Schema registry and compatibility configured
- [ ] Versioning strategy defined

### Topology
- [ ] Topic/queue structure designed
- [ ] Partitioning strategy defined
- [ ] Routing and filtering designed
- [ ] Consumer group structure planned

### Reliability
- [ ] Delivery semantics defined (at-least-once, exactly-once)
- [ ] Dead letter queues planned for all consumers
- [ ] Retry and backoff strategy designed
- [ ] Monitoring and alerting defined

### Operations
- [ ] Consumer lag monitoring planned
- [ ] Error rate monitoring planned
- [ ] Throughput monitoring planned
- [ ] Operations runbook provided

## Scoring Rubric

| Criterion | Weight | Pass Threshold |
|-----------|--------|---------------|
| Event Discovery | 15% | 100% |
| Broker Selection | 20% | >= 90% |
| Schema Design | 20% | 100% |
| Topology | 15% | >= 90% |
| Reliability | 20% | 100% |
| Operations | 10% | >= 85% |
| **Overall** | **100%** | **>= 95%** |
