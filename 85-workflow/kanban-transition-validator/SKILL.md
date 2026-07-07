---
name: kanban-transition-validator
description: Validates all Kanban task state transitions - guards, preconditions, and invariants for every valid state-to-state transition. Replaces 32 individual validate-*-to-* skills.
author: "Prateek"
type: workflow
status: production
priority: critical
execution_cost: low
---

# Kanban Transition Validator

## Validation Pattern
Every transition must pass these checks:
1. Source state matches current task state
2. Target state is reachable (see kanban-state-machine)
3. All preconditions for the target state are met
4. No invariants are violated
5. Task has required metadata for target state

## Preconditions by Target State
- **Ready**: Requirements documented, acceptance criteria defined
- **Todo**: Assigned owner, estimated effort, dependencies resolved
- **In Progress**: Developer capacity available, branch created
- **In Review**: PR submitted, all checks passing
- **Testing**: Test environment ready, test cases defined
- **Document**: Feature complete, tested
- **Done**: Documentation complete, stakeholders signed off
- **Blocked**: Blocker identified and documented
- **Breakdown**: Task is large enough to warrant splitting

## Rejection Reasons
- Transition not in allowed map
- Preconditions not met
- Invariant violation
- Missing required metadata

## Usage
Call this skill whenever validating a task state transition. Requires current state and target state as input.