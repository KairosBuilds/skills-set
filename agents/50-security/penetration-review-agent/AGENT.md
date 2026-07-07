---
name: penetration-review-agent
version: 1.0.0
status: production
priority: high
execution_cost: high
confidence_level: 85
owner: security-team
compatibility:
  opencode: ">=2.0.0"
  languages: ["All"]
  frameworks: ["Burp Suite", "Metasploit"]
  platforms: ["linux", "darwin", "windows"]
---

# Penetration Review Agent

Coordinates and reviews penetration testing activities across the security landscape. Integrates findings from all security scanners to produce a comprehensive penetration test report.
