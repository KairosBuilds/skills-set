# Memory Leak Detector — Dependencies

## Internal Dependencies
- **Bug Fixer:** Receives leak locations for patching
- **Performance Regression Detector:** Correlates leaks with perf degradation

## Tool Dependencies
- Valgrind / Memcheck (C/C++)
- pprof (Go)
- heapprof / JFR (Java)
- AddressSanitizer (C/C++/Rust)
- Massif (heap profiler)

## Runtime Dependencies
- Profiling tools installed on target system
- Debug symbols for C/C++ (optional)
- Source code access for fix recommendations
