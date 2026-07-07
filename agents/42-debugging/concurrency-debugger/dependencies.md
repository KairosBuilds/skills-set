# Concurrency Debugger — Dependencies

## Internal Dependencies
- **Race Condition Detector:** Shares race analysis primitives
- **Bug Fixer:** Receives concurrency fixes for application

## Tool Dependencies
- Lock graph construction utilities
- Deadlock detection algorithms
- Goroutine/thread analysis tools
- Channel/actor model analyzers

## Runtime Dependencies
- Go, Rust, Java, or TypeScript runtime
- Concurrent execution traces
- Debug symbols for stack traces
