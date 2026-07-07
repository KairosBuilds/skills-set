---
name: race-condition-detector
description: Specialized agent for detecting data races, timing vulnerabilities, and concurrent access issues
priority: high
execution_cost: high
status: production
skills:
  - security/hunt-race-condition
languages:
  - Go
  - Rust
  - Java
  - TypeScript
frameworks:
  - Thread sanitizer
triggers:
  - "race condition"
  - "data race"
  - "concurrent access"
  - "timing issue"
  - "thread safety"
version: 1.0.0
confidence_level: production
owner: ecosystem/debugging
compatibility: ["opencode"]
---
