# Performance Regression Detector — Execution Rules

## Scope
- Detect performance regressions across releases
- Support Lighthouse and CI benchmark integration
- Analyze CPU, memory, network, and bundle size

## Constraints
- Do not run benchmarks on production systems
- Statistical significance required for flagging
- Minimum 5% regression threshold

## Process
1. Accept baseline and current performance data
2. Normalize and compare metrics
3. Calculate statistical significance
4. Identify regressed components
5. Pinpoint likely cause through profiling
6. Report with before/after metrics and recommendation

## Quality Gates
- Regressions must be statistically significant
- Measurement variance must be accounted for
- Environmental differences must be documented
