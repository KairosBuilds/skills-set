# Legacy Modernizer Quality Checklist

## Pre-Delivery Validation

### Assessment Completeness
- [ ] Legacy system fully assessed (architecture, code quality, dependencies)
- [ ] Business-critical components identified
- [ ] Risks documented and quantified
- [ ] Baseline metrics established

### Strategy Definition
- [ ] Target architecture clearly defined
- [ ] Migration pattern chosen with rationale
- [ ] Migration sequence determined
- [ ] Success criteria defined per phase

### Migration Pattern
- [ ] Strangler fig interception layer designed
- [ ] Anti-corruption layer designed (if needed)
- [ ] Data migration strategy defined
- [ ] API coexistence approach documented

### Phased Plan
- [ ] Migration phases clearly defined
- [ ] Each phase has clear scope and deliverables
- [ ] Feature parity verification planned per phase
- [ ] Rollback procedures for each phase
- [ ] Timeline with milestones

### Risk Management
- [ ] Risk matrix completed
- [ ] Mitigation strategies for each risk
- [ ] Rollback plans tested (or plan to test)
- [ ] Communication plan for stakeholders

### Data Migration
- [ ] Data mapping between old and new schemas
- [ ] Data validation strategy defined
- [ ] Reconciliation process planned
- [ ] Data retention policy defined for legacy

## Scoring Rubric

| Criterion | Weight | Pass Threshold |
|-----------|--------|---------------|
| Assessment | 15% | 100% |
| Strategy | 20% | >= 90% |
| Migration Pattern | 20% | >= 90% |
| Phased Plan | 20% | 100% |
| Risk Management | 15% | 100% |
| Data Migration | 10% | >= 90% |
| **Overall** | **100%** | **>= 95%** |
