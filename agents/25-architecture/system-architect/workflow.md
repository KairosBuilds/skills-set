# System Architect Workflow

## Standard Design Flow

### Phase 1: Requirements Analysis
1. Review system requirements and SLAs
2. Identify scale requirements (users, data volume, throughput)
3. Define reliability targets (uptime, RPO, RTO)
4. Map constraints (budget, team, timeline)

### Phase 2: High-Level System Design
1. Define system boundaries
2. Identify major components and their responsibilities
3. Design inter-component communication patterns
4. Create system context diagram

### Phase 3: Scalability Design
1. Determine scaling model (horizontal/vertical)
2. Design load distribution strategy
3. Plan data partitioning strategy (sharding, replication)
4. Identify bottlenecks and mitigation strategies

### Phase 4: Reliability Design
1. Design redundancy and failover mechanisms
2. Define circuit breaker and retry policies
3. Plan disaster recovery strategy
4. Establish SLAs and SLOs for each component

### Phase 5: Performance Modeling
1. Estimate throughput and latency requirements
2. Identify critical paths and optimize
3. Design caching strategy
4. Plan for capacity and growth

### Phase 6: Operational Design
1. Design observability stack (metrics, logs, traces)
2. Define deployment and release strategy
3. Plan incident response procedures
4. Document runbooks

### Phase 7: Documentation & Review
1. Compile system architecture document
2. Include ADRs for key decisions
3. Present for stakeholder review
4. Iterate based on feedback

## Output Template

```
1. System Overview
2. Architecture Diagram
3. Component Specifications
4. Scalability Model
5. Reliability Design
6. Performance Characteristics
7. Operational Design
8. SLA/SLO Definitions
9. Capacity Plan
10. Disaster Recovery Plan
11. Monitoring & Observability
12. ADRs
```
