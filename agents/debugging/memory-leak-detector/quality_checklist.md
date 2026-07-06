# Memory Leak Detector — Quality Checklist

## Pre-Analysis
- [ ] Profiling tool data is available (Valgrind, pprof, etc.)
- [ ] Source code is accessible for allocation site analysis
- [ ] Application runtime environment is documented

## Analysis
- [ ] All allocation sites are identified
- [ ] Matching deallocation sites are confirmed or missing
- [ ] Reference cycles are detected in managed languages
- [ ] Ownership and borrowing rules are verified (Rust)
- [ ] Weak reference usage is checked

## Quantification
- [ ] Leak size per allocation site is measured
- [ ] Growth rate is calculated
- [ ] Time to OOM is estimated
- [ ] Severity is assigned based on impact

## Output
- [ ] Each leak has a confirmed allocation backtrace
- [ ] Fix recommendation includes code example
- [ ] Testing strategy for leak verification is provided
- [ ] False positives are explicitly noted
