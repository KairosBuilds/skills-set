# Concurrency Debugger — Quality Checklist

## Pre-Analysis
- [ ] Concurrent code or execution trace is available
- [ ] Deadlock/livelock/starvation symptoms are described
- [ ] Thread, goroutine, or task count is known

## Analysis
- [ ] All execution contexts (goroutines, threads, tasks) are mapped
- [ ] Lock graph is constructed and checked for cycles
- [ ] Wait chains are traced for blocked contexts
- [ ] Channel/actor buffer states are analyzed
- [ ] Starvation or unfair scheduling is detected

## Verification
- [ ] Deadlock cycles are fully mapped with evidence
- [ ] Contention points are identified with access frequency
- [ ] Cancellation and timeout patterns are checked

## Output
- [ ] Concurrency issue type is correctly classified
- [ ] Lock graph or wait chain visualization is provided
- [ ] Fix recommendation preserves correctness guarantees
- [ ] Performance impact of the fix is estimated
