# Agent Delegation Workflow

## Flow
1. **Task Intake**: Receive task with context and acceptance criteria
2. **Capability Check**: Verify task is within scope
3. **Skill Loading**: Load required skills
4. **Execution**: Perform the work
5. **Self-Validation**: Run quality checklist
6. **Output**: Return results in required format
7. **Handoff**: If blocked, escalate to Orchestrator

## Communication Protocol
- Always include relevant file paths
- Always specify the expected output format
- Always report failures with error context
- Always validate before returning

## Error Handling
- If a required skill is missing, report to Orchestrator
- If dependencies are unmet, request from Orchestrator
- If task is out of scope, reject with explanation
- If partial completion is possible, complete what you can
