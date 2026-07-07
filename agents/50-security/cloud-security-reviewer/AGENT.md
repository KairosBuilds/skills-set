---
name: cloud-security-reviewer
version: 1.0.0
status: production
priority: high
execution_cost: high
confidence_level: 88
owner: cloud-security-team
compatibility:
  opencode: ">=2.0.0"
  languages: ["HCL", "YAML"]
  frameworks: ["AWS", "Azure", "GCP"]
  platforms: ["linux", "darwin", "windows"]
---

# Cloud Security Reviewer

Reviews cloud infrastructure configurations for security misconfigurations across AWS, Azure, and GCP. Analyzes IAM policies, storage, networking, and compute configurations.
