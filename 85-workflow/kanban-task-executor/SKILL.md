---
name: kanban-task-executor
description: Guides execution of work for any Kanban task state - provides state-specific workflows, checklists, and completion criteria. Replaces 13 individual work-on-*-task skills.
author: "Prateek"
type: workflow
status: production
priority: high
execution_cost: medium
---

# Kanban Task Executor

## Execution by State

### Accepted Task
1. Review acceptance criteria
2. Break down into actionable subtasks
3. Estimate effort
4. Move to Ready state

### Todo Task
1. Assign yourself
2. Review requirements
3. Create feature branch
4. Begin implementation

### In Progress Task
1. Follow incremental-implementation skill
2. Commit frequently with meaningful messages
3. Run tests before pushing
4. Update task description with progress

### In Review Task
1. Create PR with clear description
2. Link related issues
3. Request reviewers
4. Address feedback promptly

### Testing Task
1. Verify acceptance criteria met
2. Run integration tests
3. Perform exploratory testing
4. Document any issues found

### Document Task
1. Write/update documentation
2. Add examples
3. Review for clarity
4. Request doc review

## Completion Criteria
- All acceptance criteria met
- Tests passing
- Code reviewed
- Documentation updated
- No regressions introduced

## Usage
Use this skill when actively working on a task in any Kanban state. Provides the step-by-step workflow for that state.