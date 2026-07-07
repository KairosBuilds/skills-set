# Microservices Architect Quality Checklist

## Pre-Delivery Validation

### Domain Analysis
- [ ] Bounded contexts clearly identified and documented
- [ ] Ubiquitous language defined
- [ ] Domain events mapped

### Service Boundaries
- [ ] Each service has clear, non-overlapping responsibility
- [ ] No shared databases between services
- [ ] Services are independently deployable
- [ ] No circular service dependencies
- [ ] Service size appropriate for business capability

### Communication
- [ ] Async communication preferred where applicable
- [ ] Synchronous calls have timeouts, retries, and circuit breakers
- [ ] Event schemas defined
- [ ] Communication matrix completed

### Data Architecture
- [ ] Per-service data ownership assigned
- [ ] Saga flows designed for multi-service transactions
- [ ] Consistency model defined per operation
- [ ] Transactional outbox pattern for reliable events

### Operations
- [ ] Service discovery mechanism defined
- [ ] API gateway / BFF strategy documented
- [ ] Monitoring and observability per service planned
- [ ] Deployment strategy defined

### Migration
- [ ] Incremental migration approach (strangler fig preferred)
- [ ] Migration sequence identified
- [ ] Success metrics defined per phase
- [ ] Rollback plan documented

## Scoring Rubric

| Criterion | Weight | Pass Threshold |
|-----------|--------|---------------|
| Domain Analysis | 15% | 100% |
| Service Boundaries | 25% | 100% |
| Communication | 20% | >= 90% |
| Data Architecture | 20% | >= 90% |
| Operations | 10% | >= 85% |
| Migration | 10% | >= 90% |
| **Overall** | **100%** | **>= 95%** |
