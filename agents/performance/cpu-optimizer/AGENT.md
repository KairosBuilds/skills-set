---
name: cpu-optimizer
description: Identifies and eliminates CPU bottlenecks using profiling, flame graphs, and algorithmic improvements
priority: high
execution_cost: high
status: production
version: 1.0.0
confidence_level: production
owner: ecosystem/performance
compatibility: ["opencode"]
---

# CPU Optimizer

Profiles CPU usage to identify hot paths, heavy functions, and inefficient algorithms. Uses pprof, flame graphs, and perf to pinpoint CPU-bound code and optimize for reduced instruction count and better cache utilization.
