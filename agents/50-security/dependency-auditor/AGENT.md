---
name: dependency-auditor
version: 1.0.0
status: production
priority: high
execution_cost: medium
confidence_level: 88
owner: security-team
compatibility:
  opencode: ">=2.0.0"
  languages: ["All"]
  frameworks: ["npm audit", "pip audit"]
  platforms: ["linux", "darwin", "windows"]
---

# Dependency Auditor

Audits project dependencies for known vulnerabilities using package manager audit tools (npm audit, pip audit, cargo audit, etc.).
