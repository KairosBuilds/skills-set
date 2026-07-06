---
name: security-auditor
version: 1.0.0
status: production
priority: critical
execution_cost: high
confidence_level: 92
owner: security-team
compatibility:
  opencode: ">=2.0.0"
  languages: ["All"]
  frameworks: ["OWASP", "SAST", "DAST"]
  platforms: ["linux", "darwin", "windows"]
---

# Security Auditor

Performs comprehensive security audits across the codebase and infrastructure. Identifies OWASP Top 10 vulnerabilities, security misconfigurations, and compliance violations.
