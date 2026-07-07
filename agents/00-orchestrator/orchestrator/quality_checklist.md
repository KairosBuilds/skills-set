# Orchestrator Quality Checklist

## Pre-Delivery Validation

### Completeness
- [ ] All subtasks completed successfully
- [ ] No component of the original request is unaddressed
- [ ] Implicit requirements (non-functional, edge cases) are addressed

### Consistency
- [ ] No internal contradictions in merged output
- [ ] Agent recommendations are compatible across domains
- [ ] Terminology is consistent throughout

### Accuracy
- [ ] Agent outputs are technically correct
- [ ] No hallucinated or unverified claims
- [ ] All code examples are syntactically valid

### Format
- [ ] Output matches requested format (document, code, diagram, etc.)
- [ ] Diagrams render correctly (Mermaid, etc.)
- [ ] Code blocks have proper language annotations

### Conflict Resolution
- [ ] All inter-agent conflicts are resolved
- [ ] Resolution decisions are documented with reasoning
- [ ] Escalated conflicts include user decision

### Context Preservation
- [ ] No context loss between agent handoffs
- [ ] Requirements are traceable through the entire workflow

## Post-Delivery Review

- [ ] User feedback received and logged
- [ ] Orchestration metrics recorded
- [ ] Routing tables updated based on outcome
- [ ] Failure modes documented for future improvement

## Scoring Rubric

| Criterion | Weight | Pass Threshold |
|-----------|--------|---------------|
| Completeness | 25% | 100% |
| Consistency | 20% | 100% |
| Accuracy | 25% | >= 90% |
| Format | 15% | 100% |
| Conflict Resolution | 15% | 100% |
| **Overall** | **100%** | **>= 95%** |
