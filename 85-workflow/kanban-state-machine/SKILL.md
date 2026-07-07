---
name: kanban-state-machine
description: Complete Kanban state machine for task lifecycle management - defines all states and valid transitions. Replaces individual kanban-state-* skills.
author: "Prateek"
type: workflow
status: production
priority: critical
execution_cost: low
---

# Kanban State Machine

## State Model
The Kanban workflow follows a directed graph:

`
Incoming -> Accepted -> Ready -> Todo -> In Progress -> In Review -> Testing -> Document -> Done
            |           |        |           |             |            |
          Icebox     Rejected  Blocked    Breakdown      Todo       In Progress
`

## States: Incoming, Accepted, Icebox, Backlog, Ready, Todo, In Progress, In Review, Testing, Document, Done, Rejected, Blocked, Breakdown

## Transition Map
- Incoming: -> Accepted, -> Icebox, -> Rejected
- Accepted: -> Ready, -> Breakdown, -> Icebox
- Ready: -> Todo, -> Breakdown, -> Rejected
- Todo: -> In Progress, -> Breakdown
- In Progress: -> In Review, -> Todo, -> Breakdown
- In Review: -> Testing, -> In Progress, -> Todo, -> Breakdown
- Testing: -> Document, -> In Progress, -> In Review
- Document: -> Done, -> In Review
- Blocked: -> Breakdown
- Breakdown: -> Ready, -> Blocked, -> Icebox, -> Rejected

## Usage
Use this skill for all kanban state-related queries - determining valid next states, understanding state semantics, or explaining the workflow model.