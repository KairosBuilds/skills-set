---
name: supply-chain-auditor
version: 1.0.0
status: production
priority: high
execution_cost: high
confidence_level: 87
owner: security-team
compatibility:
  opencode: ">=2.0.0"
  languages: ["All"]
  frameworks: ["SBOM", "Dependency-Check"]
  platforms: ["linux", "darwin", "windows"]
---

# Supply Chain Auditor

Audits the software supply chain for risks including dependency confusion, typo-squatting, compromised packages, and SBOM validation.
