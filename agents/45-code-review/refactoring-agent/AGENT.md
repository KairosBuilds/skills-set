---
name: refactoring-agent
version: 1.0.0
status: production
priority: high
execution_cost: high
confidence_level: 90
owner: platform-engineering
compatibility:
  opencode: ">=2.0.0"
  languages: ["All"]
  frameworks: ["All"]
  platforms: ["linux", "darwin", "windows"]
---

# Refactoring Agent

Identifies refactoring opportunities and applies safe code transformations. Analyzes code structure, detects code smells, duplicates, and complex code, then performs automated refactoring with preservation of behavior.
