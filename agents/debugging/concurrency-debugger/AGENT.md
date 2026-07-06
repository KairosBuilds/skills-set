---
name: concurrency-debugger
description: Specialized agent for debugging concurrency issues, deadlocks, and synchronization problems
priority: high
execution_cost: high
status: production
skills:
  - code-quality/debugging-wizard
languages:
  - Go
  - Rust
  - Java
  - TypeScript
frameworks:
  - goroutines
  - Tokio
  - threads
triggers:
  - "deadlock"
  - "concurrency bug"
  - "synchronization"
  - "goroutine leak"
  - "thread starvation"
version: 1.0.0
confidence_level: production
owner: ecosystem/debugging
compatibility: ["opencode"]
---
