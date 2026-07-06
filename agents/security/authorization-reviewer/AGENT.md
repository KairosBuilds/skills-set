---
name: authorization-reviewer
version: 1.0.0
status: production
priority: critical
execution_cost: high
confidence_level: 91
owner: security-team
compatibility:
  opencode: ">=2.0.0"
  languages: ["All"]
  frameworks: ["RBAC", "ABAC", "ACL"]
  platforms: ["linux", "darwin", "windows"]
---

# Authorization Reviewer

Reviews authorization implementations for privilege escalation, broken access control, IDOR, and role/permission misconfigurations.
