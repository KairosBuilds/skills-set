# Memory Leak Detector — Supported Frameworks

## Memory Profiling Tools
- **Valgrind** — Memcheck, Massif, DHAT for C/C++/Rust
- **heapprof** — Java heap profiling
- **pprof** — Go heap profiling

## Allocator Support
- **C++** — new/delete, malloc/free, smart pointers (shared_ptr, unique_ptr)
- **Rust** — Box, Vec, Rc, Arc, allocator API
- **Go** — GC analysis, heap object tracking
- **Java** — GC roots, heap analysis, reference types

## Frameworks with Leak Awareness
- **Android** — Activity/Fragment lifecycle, context leaks
- **Spring** — Bean lifecycle, request scope
- **React** — Component lifecycle, closure capture
- **Node.js** — EventEmitter listeners, timer leaks
