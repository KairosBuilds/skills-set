# Repository Mapper Quality Checklist

## Pre-Delivery Validation

### Scan Completeness
- [ ] All source files in scope analyzed
- [ ] Generated files excluded
- [ ] Vendor dependencies identified
- [ ] Configuration files included

### Dependency Analysis
- [ ] All internal dependencies extracted
- [ ] External dependencies cataloged
- [ ] Dependency direction tracked
- [ ] Circular dependencies identified

### Boundary Analysis
- [ ] Module boundaries mapped
- [ ] Boundary violations identified
- [ ] Layering violations detected
- [ ] Cohesion/coupling metrics provided

### Visualizations
- [ ] Directory tree included
- [ ] Dependency graph generated
- [ ] Graph is clear and navigable
- [ ] Color-coding/grouping used for clarity

### Recommendations
- [ ] Actionable insights provided
- [ ] Issues classified by severity
- [ ] Recommendations prioritized
- [ ] Estimated effort mentioned

## Scoring Rubric

| Criterion | Weight | Pass Threshold |
|-----------|--------|---------------|
| Scan Completeness | 20% | 100% |
| Dependency Analysis | 25% | >= 90% |
| Boundary Analysis | 20% | >= 90% |
| Visualizations | 20% | >= 85% |
| Recommendations | 15% | >= 90% |
| **Overall** | **100%** | **>= 95%** |
