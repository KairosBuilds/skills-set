---
name: performance-regression-detector
description: Specialized agent for detecting performance regressions and degradation across releases
priority: high
execution_cost: medium
status: production
skills:
  - Lighthouse
  - CI benchmarks
languages:
  - All
frameworks:
  - Lighthouse
triggers:
  - "performance regression"
  - "speed drop"
  - "slowdown"
  - "latency increase"
  - "benchmark decline"
version: 1.0.0
confidence_level: production
owner: ecosystem/debugging
compatibility: ["opencode"]
---
