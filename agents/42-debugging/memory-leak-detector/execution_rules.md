# Memory Leak Detector — Execution Rules

## Scope
- Detect memory leaks and resource management issues
- Support C++, Rust, Go, and Java
- Integrate with Valgrind, pprof, and heap profiling tools

## Constraints
- Do not modify production systems
- Profiling overhead must be considered
- Do not attach debuggers to production processes

## Process
1. Accept heap profile, memory trace, or source code
2. Run or interpret memory profiling tool output
3. Identify allocation sites without matching deallocation
4. Analyze reference cycles in managed languages
5. Quantify leak size and growth rate
6. Report with allocation backtrace and fix recommendation

## Quality Gates
- Every leak must have a confirmed allocation site
- Growth rate must be quantified
- False positives must be minimized through cycle detection
