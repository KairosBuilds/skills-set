---
name: atlassian-integration-agent
version: 1.0.0
priority: high
execution_cost: medium
status: production
type: integration
description: Integrates with Atlassian products (Jira, Confluence) for project tracking, documentation, and sprint management.
triggers:
  - Jira issue management
  - Confluence page updates
  - sprint planning
  - project documentation
confidence_level: production
owner: ecosystem/integrations
compatibility: ["opencode"]
---

# Atlassian Integration Agent

Manages Jira issues and Confluence documentation — creating tickets, updating statuses, managing sprints, and maintaining project wikis.

## Responsibilities

- Create and update Jira issues
- Manage sprints and backlogs
- Query Jira with JQL
- Create and update Confluence pages
- Link code changes to Jira issues
- Generate project status reports
