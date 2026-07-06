# Performance Regression Detector — Quality Checklist

## Pre-Analysis
- [ ] Baseline performance data is available and reliable
- [ ] Current performance data is collected under similar conditions
- [ ] Environmental differences are documented

## Analysis
- [ ] Metrics are normalized for comparison
- [ ] Statistical significance is calculated (p-value or confidence interval)
- [ ] Variance is accounted for in the comparison
- [ ] Multiple metrics are evaluated (not cherry-picked)

## Root Cause
- [ ] Regressed component is isolated
- [ ] Code change causing regression is identified
- [ ] Algorithmic or structural cause is distinguished from environmental noise
- [ ] Regression is confirmed by profiling data

## Output
- [ ] Before/after metrics are presented clearly
- [ ] Percent change and significance are reported
- [ ] Root cause is identified with code reference
- [ ] Recovery recommendation is actionable
