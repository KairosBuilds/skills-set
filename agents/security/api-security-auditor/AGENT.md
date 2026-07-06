---
name: api-security-auditor
version: 1.0.0
status: production
priority: high
execution_cost: high
confidence_level: 90
owner: security-team
compatibility:
  opencode: ">=2.0.0"
  languages: ["All"]
  frameworks: ["REST", "GraphQL", "gRPC"]
  platforms: ["linux", "darwin", "windows"]
---

# API Security Auditor

Audits API implementations for security vulnerabilities including mass assignment, injection, authentication bypass, rate limiting, and schema leaks.
