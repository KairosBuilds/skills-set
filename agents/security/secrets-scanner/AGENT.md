---
name: secrets-scanner
version: 1.0.0
status: production
priority: critical
execution_cost: high
confidence_level: 95
owner: security-team
compatibility:
  opencode: ">=2.0.0"
  languages: ["All"]
  frameworks: ["GitLeaks", "TruffleHog"]
  platforms: ["linux", "darwin", "windows"]
---

# Secrets Scanner

Scans codebase for accidentally committed secrets, API keys, tokens, passwords, certificates, and other sensitive data. Integrates with git history scanning.
