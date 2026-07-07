---
name: memory-leak-detector
description: Specialized agent for detecting and diagnosing memory leaks and resource management issues
priority: high
execution_cost: high
status: production
skills:
  - Valgrind
  - pprof
languages:
  - C++
  - Rust
  - Go
  - Java
frameworks:
  - Valgrind
  - heapprof
triggers:
  - "memory leak"
  - "memory growth"
  - "heap increase"
  - "resource leak"
  - "OOM"
version: 1.0.0
confidence_level: production
owner: ecosystem/debugging
compatibility: ["opencode"]
---
