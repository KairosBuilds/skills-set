---
name: context-management
description: Strategies and patterns for managing LLM context windows effectively. Covers context budgeting, token optimization, retrieval-augmented generation, memory systems, progressive disclosure, and session persistence. Use when context window is limited, responses are incomplete, or agent forgets earlier instructions. Not for writing code or reviewing diffs.
license: MIT
compatibility: opencode
metadata:
  author: "Prateek"
  version: "1.0.0"
  domain: opencode
  triggers: context, context window, token limit, memory, remember, forget, session persistence
  role: standard
  scope: productivity
  output-format: reference
  related-skills: prompt-engineering, progressive-disclosure, opencode-skill-creation, opencode-configs
---

# Context Management

Strategies for managing LLM context windows effectively in AI-assisted development.

## Core Concepts

### Context Window Budget
```
[System/Rules]     ~20% — Persistent instructions, project rules
[Conversation]     ~30% — Current session history
[Files/Data]       ~40% — Files being read or modified
[Output]           ~10% — Space for generating responses
```

### Token Optimization Strategies

| Strategy | Savings | Tradeoff |
|----------|---------|----------|
| Remove verbose comments | 5-15% | Less explanatory code |
| Use shorter variable names in examples | 2-5% | Less readable examples |
| Reference files by path, not content | 10-40% | Requires file read tool |
| Summarize past decisions | 15-25% | Loses nuance |
| Chunk large files | 20-50% | Breaks cross-file patterns |
| Use bullet points over prose | 10-20% | Less natural language |
| Remove irrelevant conversation history | 30-50% | Loses chain of thought |

## Techniques

### Progressive Disclosure
Start with a minimal prompt. Expand detail only when needed. Use reference files for deep context:

```
Initial: "Implement a React component for [purpose]"
If needed: "See .claude/references/component-patterns.md for our conventions"
```

### Memory Systems
- **Short-term memory**: Current conversation history
- **Long-term memory**: AGENTS.md, CLAUDE.md, project rules
- **Working memory**: Current task context, open files
- **Reference memory**: Skills, references, documentation

### Retrieval-Augmented Generation (RAG)
For large codebases:
1. Identify the relevant files first (grep, glob, read)
2. Only include relevant sections in context
3. Use summaries for peripheral files
4. Reference by path, quote only essential lines

### Session Persistence
- Save planning decisions to docs/ or plans/ directory
- Update AGENTS.md with learned project patterns
- Use CHANGELOG.md to track what changed between sessions
- Write handoff documents for multi-session work

## Progressive Disclosure Hierarchy

```
Level 0: Task prompt (what to do)
Level 1: AGENTS.md / system instructions (how to behave)
Level 2: Skill files (reusable workflows)
Level 3: Reference files (deep domain knowledge)
Level 4: Full codebase (implementation details)
```

Load only as deep as needed for the current task.

## Anti-Patterns

| Anti-Pattern | Problem | Fix |
|---|---|---|
| Full file reads for every reference | Wastes context | Read only relevant sections |
| Repeating instructions every session | Redundant | Store in AGENTS.md |
| Keeping all conversation history | Rapid context exhaustion | Summarize and truncate |
| No project-level instructions | Inconsistent behavior | Create AGENTS.md |
| Overloaded AGENTS.md | Important rules diluted | Use layered rules |
