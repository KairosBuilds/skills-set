# Race Condition Detector — Dependencies

## Internal Dependencies
- **Concurrency Debugger:** Extended analysis for complex race scenarios
- **Bug Fixer:** Receives race locations for synchronization fixes

## Tool Dependencies
- ThreadSanitizer (Go, Rust, C++, Java)
- Go race detector
- Java Happens-Before analysis
- Lock validation tools

## Runtime Dependencies
- Go, Rust, Java, or TypeScript runtime
- Race detection enabled builds
- Stress testing framework for reproduction
