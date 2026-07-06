# Examples

## Agent Builder

### Example 1: Agent Directory Structure
```
my-agent/
  AGENT.md
  metadata.yaml
  config.json
  execution_rules.md
  workflow.md
  examples.md
  dependencies.md
  supported_skills.md
  supported_languages.md
  supported_frameworks.md
  limitations.md
  quality_checklist.md
```

### Example 2: AGENT.md Frontmatter
```yaml
---
name: My Agent
version: 1.0.0
status: production
priority: high
execution_cost: medium
confidence_level: high
owner: ai-team
compatibility: opencode
---
```

### Example 3: MCP Server Config
```json
{
  "mcpServers": {
    "my-server": {
      "command": "node",
      "args": ["server.js"],
      "env": {}
    }
  }
}
```
