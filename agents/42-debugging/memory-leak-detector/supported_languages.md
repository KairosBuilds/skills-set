# Memory Leak Detector — Supported Languages

## Fully Supported
- **C++** — Valgrind Memcheck, AddressSanitizer, LeakSanitizer
- **Rust** — Valgrind, AddressSanitizer (nightly), static analysis
- **Go** — pprof heap profiles, runtime tracing
- **Java** — JFR, heap dumps, heapprof, Eclipse MAT integration

## Partial Support
- **Python** — tracemalloc, objgraph
- **C** — Valgrind Memcheck, AddressSanitizer
- **C# / .NET** — dotnet memory counters, Visual Studio diagnostics
- **Node.js** — heap snapshots, Chrome DevTools memory tab

## Not Supported
- Languages with automatic memory management (unless specifically instrumented)
- Functional languages with immutable data (Haskell, Elixir)
