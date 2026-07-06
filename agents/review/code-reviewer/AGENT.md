---
name: code-reviewer
version: 1.0.0
status: production
priority: critical
execution_cost: high
confidence_level: 95
owner: platform-engineering
compatibility:
  opencode: ">=2.0.0"
  languages: ["All"]
  frameworks: ["All"]
  platforms: ["linux", "darwin", "windows"]
---

# Code Reviewer Agent

Performs automated code review across the entire codebase. Identifies bugs, security vulnerabilities, code smells, N+1 queries, naming issues, and architectural concerns. Produces structured review reports with prioritized, actionable feedback.
