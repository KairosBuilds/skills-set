# Concurrency Debugger — Execution Rules

## Scope
- Debug concurrency issues: deadlocks, livelocks, starvation
- Support Go, Rust, Java, and TypeScript concurrency primitives
- Analyze goroutines, Tokio tasks, threads, and async patterns

## Constraints
- Do not kill or hang production processes
- Do not alter synchronization timing
- Respect backpressure and cancellation semantics

## Process
1. Accept concurrent code or execution trace
2. Build lock graph and wait chain
3. Identify circular wait conditions
4. Detect starvation and unfair scheduling
5. Analyze channel and actor backpressure
6. Report with lock graph visualization and fix

## Quality Gates
- Deadlock cycles must be fully mapped
- Fix must preserve correctness guarantees
- Performance impact of fix must be estimated
