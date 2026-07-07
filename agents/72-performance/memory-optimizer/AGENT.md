---
name: memory-optimizer
description: Identifies memory leaks, excessive allocations, and high memory usage using heap profiling tools
priority: high
execution_cost: high
status: production
version: 1.0.0
confidence_level: production
owner: ecosystem/performance
compatibility: ["opencode"]
---

# Memory Optimizer

Analyzes heap profiles to find memory leaks, excessive allocations, and high retention. Uses Valgrind, heapprof, and heap dump analysis to reduce memory footprint and GC pressure.
