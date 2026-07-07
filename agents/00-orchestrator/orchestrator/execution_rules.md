# Orchestrator Execution Rules

## Routing Rules

1. **Primary-first** — Always route to the primary agent for a task type before considering fallbacks
2. **Capability match** — Only route to agents whose declared skills cover >= 80% of task requirements
3. **Load balancing** — Distribute concurrent subtasks across available agents; avoid overloading single agent
4. **Dependency ordering** — Execute dependent tasks strictly after prerequisite tasks complete
5. **Parallel execution** — Execute independent subtasks concurrently where possible

## Conflict Resolution Rules

1. **Priority override** — Higher-priority agent output takes precedence on conflicting recommendations
2. **Specificity wins** — More domain-specific agent (narrower skill scope) overrides generalist
3. **Recency bias** — Most recent analysis supersedes earlier ones; log the reasoning
4. **Escalation** — If rules 1-3 cannot resolve, generate a comparative analysis and present to user
5. **Audit** — Every conflict and resolution is recorded with: agents involved, conflict nature, resolution rule applied, timestamp

## Quality Rules

1. **Validation required** — Every merged output must pass the quality checklist before delivery
2. **Confidence gate** — Do not deliver outputs below confidence threshold (0.8); request revision or re-route
3. **Consistency check** — Verify merged output has no internal contradictions from different agents
4. **Completeness check** — Verify all subtask outputs are incorporated; nothing omitted
5. **Format compliance** — Verify output matches requested format (document, code, diagram, etc.)

## Communication Rules

1. **Context preservation** — Pass all relevant context to downstream agents; never drop context silently
2. **No redundancy** — Avoid passing duplicate context that forces agents to re-parse known information
3. **Clear handoffs** — Each agent handoff includes: task description, context, expected output, and deadline
4. **Status reporting** — Report orchestration progress to user at meaningful milestones

## Error Handling Rules

1. **Agent failure** — If primary agent fails, retry once; if retry fails, route to fallback agent
2. **Timeout** — If agent exceeds timeout, consider it failed and route to fallback
3. **Partial results** — If some subtasks succeed and others fail, deliver partial results with clear failure documentation
4. **Fatal error** — If orchestration cannot proceed (no available agents, unrecoverable conflict), escalate to user
