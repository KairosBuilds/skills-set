# Runtime Error Specialist — Limitations

## Detection Limitations
- Cannot prevent all runtime errors — only identifies patterns
- Requires error context (stack trace, input) for accurate diagnosis
- Cannot reproduce intermittent runtime errors
- Some runtime errors depend on environmental state

## Scope Limitations
- Cannot fix architectural issues that cause runtime errors
- External service errors (network, API) are diagnosed but not fixed
- Memory-related runtime errors may overlap with Memory Leak Detector
- Concurrency-related runtime errors should be escalated to Concurrency Debugger

## Language-Specific Limitations
- Unsafe code blocks (C#, Rust) bypass normal type safety
- Dynamic typing languages have inherently higher runtime error rates
- Reflection-heavy code makes static analysis difficult
