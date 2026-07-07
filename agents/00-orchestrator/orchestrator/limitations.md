# Orchestrator Limitations

## Functional Limitations

1. **No direct domain execution** — Orchestrator does not write code, design databases, or perform specialized domain tasks directly; it routes to specialists
2. **Agent dependency** — Orchestrator quality is bounded by the capabilities of the agents it routes to
3. **Context window limits** — Very large multi-agent workflows may exceed shared context capacity
4. **No real-time coordination** — Orchestrator operates on a request-response model, not continuous real-time coordination
5. **Conflict resolution subjectivity** — Priority and specificity rules may not always produce optimal resolutions

## Performance Limitations

1. **Sequential bottleneck** — Tasks with deep dependency chains increase wall-clock time
2. **Overhead** — Multi-agent orchestration adds routing and coordination overhead compared to single-agent execution
3. **Concurrency ceiling** — Limited by available agents and execution environment resources

## Scope Limitations

1. **Cannot operate without agent registry** — Agent capability discovery is a prerequisite
2. **Limited to defined agent skill boundaries** — Cannot route to capabilities not declared by any agent
3. **No autonomous agent creation** — Orchestrator cannot create new agents on demand

## Known Edge Cases

1. **Circular dependencies** — Subtask dependency graphs must be acyclic; orchestrator cannot handle circular dependencies
2. **Identical agent conflicts** — When two agents with same priority and specificity disagree, escalation is always required
3. **Partial agent failure** — When only some subtasks complete, orchestrator delivers partial results with caveats
4. **Agent unavailability** — No graceful degradation if all candidates for a subtask are unavailable
