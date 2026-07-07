# Race Condition Detector — Quality Checklist

## Pre-Analysis
- [ ] Source code with concurrent access patterns is provided
- [ ] ThreadSanitizer or race detector output is available (if applicable)
- [ ] Go race flag or Java instrumentation is enabled

## Analysis
- [ ] All shared mutable state is identified
- [ ] Read/write access patterns are mapped per variable
- [ ] Synchronization primitive coverage is verified
- [ ] Happens-before relationships are traced
- [ ] Conflicting access pairs are identified

## Verification
- [ ] Each race is reproducible
- [ ] Benign races are distinguished from harmful ones
- [ ] Exploitability or impact is assessed
- [ ] Timing window is characterized

## Output
- [ ] Conflicting access pairs include file and line numbers
- [ ] Thread and stack trace is provided for each access
- [ ] Fix recommendation is specific and actionable
- [ ] Fix does not introduce deadlocks
