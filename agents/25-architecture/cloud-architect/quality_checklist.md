# Cloud Architect Quality Checklist

## Pre-Delivery Validation

### Requirements Coverage
- [ ] All application requirements addressed
- [ ] Compliance and regulatory requirements identified
- [ ] Success criteria defined

### Architecture
- [ ] Architecture follows Well-Architected Framework (all 6 pillars)
- [ ] Network topology designed with security best practices
- [ ] Compute architecture matches workload characteristics
- [ ] Storage and data architecture designed
- [ ] High availability and fault tolerance designed

### Security
- [ ] IAM follows least privilege
- [ ] Encryption at rest and in transit
- [ ] Network segmentation and isolation
- [ ] Secrets management strategy defined
- [ ] Logging and monitoring for security events

### Migration (if applicable)
- [ ] Migration strategy chosen per workload
- [ ] Migration waves defined with dependencies
- [ ] Cutover and rollback procedures documented
- [ ] Testing strategy defined

### Cost
- [ ] Cost estimates provided
- [ ] Optimization opportunities identified
- [ ] Auto-scaling strategy defined
- [ ] Tagging strategy for cost allocation

### Operations
- [ ] DR and backup strategy defined
- [ ] RPO/RTO targets documented
- [ ] Monitoring and alerting strategy
- [ ] Operations runbooks created

## Scoring Rubric

| Criterion | Weight | Pass Threshold |
|-----------|--------|---------------|
| Requirements | 10% | 100% |
| Architecture | 25% | >= 90% |
| Security | 20% | 100% |
| Migration | 15% | >= 90% |
| Cost | 15% | >= 85% |
| Operations | 15% | >= 90% |
| **Overall** | **100%** | **>= 95%** |
