# Race Condition Detector — Execution Rules

## Scope
- Detect data races and concurrent access violations
- Support Go, Rust, Java, and TypeScript
- Use thread sanitizer and happens-before analysis

## Constraints
- Do not inject race conditions to test
- Do not modify production concurrent code without verification
- Respect existing synchronization primitives

## Process
1. Accept source code or concurrency trace
2. Analyze shared memory access patterns
3. Identify unsynchronized read-write or write-write pairs
4. Map happens-before relationships
5. Classify race severity and exploitability
6. Report with access pair locations and fix strategy

## Quality Gates
- Each race must be reproducible
- False positives must be explicitly noted
- Fix must not introduce deadlocks
