# Performance Regression Detector — Workflow

1. **Input Reception**
   - Baseline and current performance metrics
   - Lighthouse reports, CI benchmark outputs
   - Profiling data (CPU, memory, network)

2. **Metric Normalization**
   - Align metrics from different sources
   - Account for environmental differences
   - Calculate variance and confidence intervals

3. **Comparison Analysis**
   - Compare each metric against baseline
   - Calculate percent change
   - Flag changes exceeding threshold (default 5%)
   - Assess statistical significance via t-test or similar

4. **Component Isolation**
   - Identify which component regressed
   - Use flame graphs or profile comparisons
   - Narrow to specific functions or pages

5. **Root Cause Analysis**
   - Examine code changes between versions
   - Identify algorithmic or structural changes
   - Check for unintended resource leaks

6. **Report**
   - Performance before/after comparison
   - Statistical significance
   - Root cause with code reference
   - Recovery recommendations
