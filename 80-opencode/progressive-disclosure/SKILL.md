---
name: progressive-disclosure
description: Design pattern for AI agent instructions and skills that starts with lean cores and reveals detail on demand. Reduces token consumption, improves initial response speed, and prevents context window overload. Use when writing agent skills, AGENTS.md files, or any instruction set for AI agents.
license: MIT
compatibility: opencode
metadata:
  author: "Prateek"
  version: "1.0.0"
  domain: opencode
  triggers: progressive disclosure, lean skills, token optimization, skill design, instruction layering
  role: standard
  scope: productivity
  output-format: reference
  related-skills: context-management, prompt-engineering, skill-authoring, opencode-skill-creation
---

# Progressive Disclosure

Design pattern for AI agent instructions that reveals detail on demand. Lean 80-line cores with routing tables to detailed references. 50% token reduction, faster initial responses.

## Core Principle

**Start minimal, expand only when needed.** The agent should load enough to answer the immediate question, not the entire knowledge base.

## Structure

### Skill Core (80-150 lines)
```
--- frontmatter ---
# Skill Name
Short description of purpose.
When to invoke this skill.

## Outcome Contract
What success looks like.

## Quick start (3-5 lines)
The most common use case.

## Routing Table
| Trigger | Mode | Detail |
|---------|------|--------|
| Simple task | Quick mode | Inline |
| Complex task | Full mode | Load references/xxx.md |
| Special case | Specialist mode | Load references/yyy.md |

## Hard Rules (5-10)
Non-negotiable constraints.

## Output Format
Minimal output template.
```

### Reference Files
```
references/
  xxx.md — Detailed workflow for mode X
  yyy.md — Deep knowledge for specialist mode
  zzz.md — Examples and templates
```

## Benefits

| Metric | Improvement |
|--------|-------------|
| Initial response tokens | 40-60% reduction |
| Time to first output | 30-50% faster |
| Context budget for conversation | 2x more room |
| Maintainability | Easier to update core vs references |
| Discoverability | Routing table makes modes obvious |

## How to Apply

### For Skills
1. Start with the core: what, when, outcome, 5-10 hard rules
2. Extract detailed workflows into references/ directory
3. Add a routing table at the top of each mode section
4. Keep core under 150 lines; references can be any length

### For AGENTS.md
1. Top section: project identity, stack, conventions (essential only)
2. Middle section: rules and patterns (moderately detailed)
3. References at bottom: deep docs, architecture, API specs

### For Rules
1. Rule name and trigger pattern
2. One-sentence rule
3. One-sentence rationale
4. Example (good/bad)
5. Reference to deeper doc if needed

## Anti-Patterns

| Anti-Pattern | Problem | Fix |
|---|---|---|
| Everything in one file | Context overload | Extract references |
| References that are too short | Don't add value | Include examples, edge cases |
| No routing table | Agent doesn't know what to load | Add trigger → mode → reference mapping |
| Core too long | Defeats purpose | Ruthlessly cut to essentials |
| Stale references | Wrong guidance | Keep in sync with core |
