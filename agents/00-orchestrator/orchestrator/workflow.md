# Orchestrator Workflow

## Standard Orchestration Flow

### Phase 1: Ingest & Parse
1. Receive user request
2. Extract: intent, domain, scope, constraints, output format, priority
3. Identify implicit requirements (non-functional, edge cases)
4. Classify task complexity: simple (single agent) vs complex (multi-agent)

### Phase 2: Decompose
1. Break complex tasks into discrete subtasks
2. Map subtask dependencies (DAG construction)
3. Identify parallelizable subtasks
4. Assign priority levels to subtasks

### Phase 3: Select & Route
1. Match each subtask to agent capabilities
2. Check agent availability and load
3. Route subtask with full context package
4. Set expectations: output format, deadline, confidence threshold

### Phase 4: Monitor & Coordinate
1. Track subtask progress
2. Handle agent failures and timeouts
3. Manage inter-agent dependencies
4. Detect and resolve conflicts as they arise

### Phase 5: Merge & Validate
1. Collect all agent outputs
2. Merge into coherent deliverable
3. Resolve inter-agent contradictions
4. Run quality checklist
5. Generate final output

### Phase 6: Deliver & Log
1. Present output to user
2. Request feedback
3. Log orchestration metrics
4. Update routing tables based on results

## Simple Task Workflow (Single Agent)

```
Parse -> Route -> Validate -> Deliver
```

## Complex Task Workflow (Multi-Agent)

```
Parse -> Decompose -> [Route A, Route B (parallel)] 
     -> [Wait for A+B] -> Route C (depends on A+B) 
     -> Merge -> Validate -> Deliver
```

## Conflict Resolution Workflow

```
Detect Conflict
    |
Log Conflict Details
    |
Apply Resolution Rules (priority/specificity/recency)
    |
If Resolved -> Update output, log resolution
    |
If Unresolved -> Generate comparison, present to user
    |
User Decision -> Update output, log decision
```

## Quality Validation Flow

```
Receive Merged Output
    |
Check against quality_checklist.md
    |
If Passes -> Deliver
    |
If Fails -> Identify failing criteria
    |
Request Revision from relevant agent(s)
    |
Re-validate -> Deliver
```
