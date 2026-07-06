# Stack Trace Analyzer — Quality Checklist

## Pre-Analysis
- [ ] Raw stack trace is complete and readable
- [ ] Source maps or symbol files are available (or noted missing)
- [ ] Language and runtime are correctly identified

## Analysis
- [ ] Stack trace format is correctly detected
- [ ] All frames are parsed and normalized
- [ ] Application frames are distinguished from library/runtime frames
- [ ] Root cause frame is correctly identified
- [ ] Chained exceptions are unwrapped to innermost cause

## Mapping
- [ ] Frame locations are mapped to source code
- [ ] Source maps are applied correctly for minified code
- [ ] Async continuations are correlated (if applicable)
- [ ] Native frames are identified (if mixed runtime)

## Output
- [ ] Annotated stack trace is clear and readable
- [ ] Root cause is stated with line number and function
- [ ] Relevant code snippets are included for context
- [ ] Fix direction is actionable
