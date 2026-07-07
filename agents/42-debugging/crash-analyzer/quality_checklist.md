# Crash Analyzer — Quality Checklist

## Pre-Analysis
- [ ] Crash data format is identified and supported
- [ ] Debug symbols or source maps are available (or noted missing)
- [ ] Application version and environment are documented

## Analysis
- [ ] Crash type is correctly classified
- [ ] Access violation address is analyzed
- [ ] Stack frames are walked to root cause
- [ ] Application code frames are distinguished from library frames
- [ ] Chained exceptions are unwrapped to innermost cause

## Root Cause
- [ ] Exact line and function of failure is identified
- [ ] Input or condition leading to crash is determined
- [ ] Crash is reproducible with the identified conditions
- [ ] Similar crash patterns are cross-referenced

## Output
- [ ] Root cause is clearly stated with evidence
- [ ] Reproduction steps are deterministic
- [ ] Fix recommendation is actionable
- [ ] Severity assessment matches crash impact
