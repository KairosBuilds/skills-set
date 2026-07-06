---
name: auto-fix-agent
version: 1.0.0
priority: high
execution_cost: medium
status: production
type: automation
description: Automatically detects and fixes code quality issues, resolves merge conflicts, and breaks edit loops using AI-powered remediation.
triggers:
  - lint error detected
  - build failure
  - merge conflict
  - edit loop detected
  - type error found
confidence_level: production
owner: ecosystem/automation
compatibility: ["opencode"]
---

# Auto-Fix Agent

Automatically resolves common code quality issues, corrects lint/type errors, fixes merge conflicts, and breaks out of repetitive edit loops.

## Responsibilities

- Auto-fix lint and formatting errors
- Resolve type conflicts
- Fix merge conflicts automatically
- Detect and break edit loops
- Apply safe automated patches
- Report fix success rates
