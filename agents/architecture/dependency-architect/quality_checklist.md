# Dependency Architect Quality Checklist

## Pre-Delivery Validation

### Discovery Completeness
- [ ] All dependencies cataloged (internal + external)
- [ ] Direct and transitive dependencies distinguished
- [ ] Dev/peer/production dependencies classified
- [ ] Version information recorded

### Structure Analysis
- [ ] Dependency graph complete and accurate
- [ ] Coupling metrics calculated (afferent, efferent, instability)
- [ ] Circular dependencies identified
- [ ] Module layering assessed

### Boundary Analysis
- [ ] Module API surfaces defined
- [ ] Boundary compliance verified
- [ ] Transitive dependency leakage identified
- [ ] Abstraction leaks documented

### Optimization Recommendations
- [ ] Issues prioritized by severity
- [ ] Refactoring strategies proposed for circular dependencies
- [ ] Boundary enforcement improvements suggested
- [ ] Dependency reduction opportunities identified

### Governance
- [ ] Dependency rules and policies defined
- [ ] Automated enforcement tools recommended
- [ ] Review process documented
- [ ] Governance policy is actionable

## Scoring Rubric

| Criterion | Weight | Pass Threshold |
|-----------|--------|---------------|
| Discovery | 15% | 100% |
| Structure Analysis | 25% | >= 90% |
| Boundary Analysis | 20% | >= 90% |
| Recommendations | 25% | >= 90% |
| Governance | 15% | 100% |
| **Overall** | **100%** | **>= 95%** |
