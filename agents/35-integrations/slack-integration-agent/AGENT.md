---
name: slack-integration-agent
version: 1.0.0
priority: low
execution_cost: low
status: stable
type: integration
description: Manages Slack messaging, notifications, and internal communications through Slack API integration.
triggers:
  - Slack notification
  - channel message
  - status update
  - team broadcast
confidence_level: stable
owner: ecosystem/integrations
compatibility: ["opencode"]
---

# Slack Integration Agent

Handles Slack communications — sending notifications, managing messages, and coordinating team updates through the Slack API.

## Responsibilities

- Send notifications to channels
- Format messages with blocks
- Manage channel subscriptions
- Handle message threading
- Integrate with other tools via webhooks
