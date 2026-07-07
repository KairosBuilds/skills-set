# Solution Architect Quality Checklist

## Pre-Delivery Validation

### Requirements Coverage
- [ ] All functional requirements addressed
- [ ] All non-functional requirements addressed (scalability, availability, latency, security, cost)
- [ ] Constraints documented and respected
- [ ] Assumptions explicitly stated

### Design Quality
- [ ] Architecture pattern clearly defined and justified
- [ ] Component boundaries are logical and maintainable
- [ ] Data flow is documented and consistent
- [ ] Cross-cutting concerns addressed
- [ ] Failure modes considered

### Technology Selection
- [ ] At least 2 alternatives evaluated per decision
- [ ] Selection criteria applied consistently
- [ ] Trade-offs documented for each choice
- [ ] Recommendations aligned with requirements

### Documentation
- [ ] ADR created for each significant decision
- [ ] Diagram(s) included and correctly rendered
- [ ] Risk assessment included
- [ ] Implementation roadmap provided
- [ ] Terminology glossary (if needed)

### Consistency
- [ ] No internal contradictions
- [ ] Terminology is consistent throughout
- [ ] Diagram matches text description

## Scoring Rubric

| Criterion | Weight | Pass Threshold |
|-----------|--------|---------------|
| Requirements Coverage | 20% | 100% |
| Design Quality | 25% | >= 90% |
| Technology Selection | 20% | >= 90% |
| Documentation | 20% | 100% |
| Consistency | 15% | 100% |
| **Overall** | **100%** | **>= 95%** |
