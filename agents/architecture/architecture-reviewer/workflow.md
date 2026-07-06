# Architecture Reviewer Workflow

## Standard Review Flow

### Phase 1: Intake
1. Receive architecture artifacts for review
2. Identify review scope and depth required
3. Gather context: project goals, constraints, stakeholders
4. Confirm review criteria and expectations

### Phase 2: Analysis
1. Review requirements coverage (functional + non-functional)
2. Evaluate architecture pattern appropriateness
3. Analyze component decomposition and boundaries
4. Review technology selection decisions
5. Examine data flow and integration patterns
6. Assess cross-cutting concerns (security, scalability, reliability)

### Phase 3: ADR Review
1. Verify all key decisions have ADRs
2. Evaluate ADR completeness and quality
3. Check consistency across ADRs
4. Validate reasoning and alternatives

### Phase 4: Risk Assessment
1. Identify architectural risks
2. Classify risks by severity and likelihood
3. Document risk mitigation recommendations
4. Highlight critical path issues

### Phase 5: Reporting
1. Compile review findings with severity ratings
2. Provide actionable recommendations
3. Document positive aspects
4. Summarize overall architecture health score

### Phase 6: Follow-up
1. Present review to stakeholders
2. Discuss findings and recommendations
3. Track resolution of critical issues
4. Offer re-review if major changes are made

## Review Report Template

```
# Architecture Review Report

## Summary
- Architecture: [name]
- Reviewer: architecture-reviewer
- Date: [date]
- Overall Assessment: [pass/conditional/fail]

## Positive Findings
1. ...

## Issues (by Severity)

### Critical
1. ...

### High
1. ...

### Medium
1. ...

### Low
1. ...

### Info
1. ...

## Risk Assessment
- Risk Matrix: [likelihood x impact]

## Recommendations (Priority Order)
1. ...

## Score Card
| Criteria | Score | Notes |
|----------|-------|-------|
| Requirements Coverage | X/10 | ... |
| Design Quality | X/10 | ... |
| ADR Quality | X/10 | ... |
| Risk Management | X/10 | ... |
| Overall | X/10 | ... |
```
