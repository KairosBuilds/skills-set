# Memory Leak Detector — Limitations

## Tool Limitations
- Profiling tools add overhead (Valgrind: 10-20x slowdown)
- Go pprof requires `import _ "net/http/pprof"` or runtime API
- Java heap dump analysis requires heap dumps to be enabled
- AddressSanitizer requires recompilation

## Detection Limitations
- Cannot detect leaks in code without profiling data
- Generational garbage collection may hide temporary leaks
- Reference cycles in managed languages require full GC root analysis
- Native memory leaks in JVM (off-heap) are harder to detect
- Cannot detect leaks in third-party binary dependencies

## Scope Limitations
- Memory fragmentation analysis requires specialized tools
- Cache-based "logical" leaks require domain knowledge
- OS-level memory leaks (kernel drivers) are out of scope
- GPU memory leaks require separate tooling
