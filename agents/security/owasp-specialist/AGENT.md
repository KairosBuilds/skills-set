---
name: owasp-specialist
version: 1.0.0
status: production
priority: critical
execution_cost: high
confidence_level: 94
owner: security-team
compatibility:
  opencode: ">=2.0.0"
  languages: ["All"]
  frameworks: ["OWASP Top 10"]
  platforms: ["linux", "darwin", "windows"]
---

# OWASP Specialist

Focused on detecting OWASP Top 10 vulnerabilities: injection, broken auth, sensitive data exposure, XXE, broken access control, XSS, deserialization, logging, SSRF.
