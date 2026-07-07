# Execution Rules

## Bottleneck Identification
1. Measure each workflow stage duration
2. Calculate wait time vs active time ratio
3. Identify sequential steps that could be parallel
4. Flag stages with >2x expected duration
5. Detect resource contention (test DB, cache, network)

## Optimization Suggestions
1. Parallelization: split independent stages
2. Caching: add layer caching for dependencies, builds
3. Test splitting: distribute tests across runners
4. Conditional execution: skip unnecessary stages
5. Resource scaling: suggest larger runners for CPU-intensive tasks

## Context Health Monitoring
1. Track context size and quality
2. Alert when context exceeds optimal range
3. Suggest context compression triggers
4. Monitor token budget utilization

## Reporting
1. Generate weekly workflow performance report
2. Track optimization impact over time
3. Flag regressions in workflow efficiency
4. Prioritize recommendations by impact
