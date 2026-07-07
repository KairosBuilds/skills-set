# Race Condition Detector — Limitations

## Detection Limitations
- Static analysis may miss races involving dynamic thread creation
- ThreadSanitizer requires code to be compiled with instrumentation
- Some races are inherently non-deterministic and hard to reproduce
- Benign races (intentional unsynchronized access) must be distinguished

## Coverage Limitations
- Requires all threads to be running during analysis
- Race detection on production workloads may have false positives
- Cross-process races (shared memory, mmap) are harder to detect
- Hardware memory ordering issues (ARM vs x86) may be missed

## Language-Specific Limitations
- Go: only detects races when `-race` flag is used
- Rust: safe Rust eliminates data races, but unsafe code may still race
- Java: happens-before analysis is complex with volatile and final fields
- TypeScript: SharedArrayBuffer races depend on browser/Node implementation
