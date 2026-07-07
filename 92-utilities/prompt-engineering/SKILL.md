---
name: prompt-engineering
description: Library of prompt engineering patterns, techniques, and best practices for getting optimal results from LLMs. Covers system prompts, few-shot learning, chain-of-thought, structured output, context management, and iteration strategies. Use when crafting prompts for AI coding tools, designing agent instructions, or optimizing LLM interactions.
license: MIT
compatibility: opencode
metadata:
  author: "Prateek"
  version: "1.0.0"
  domain: utilities
  triggers: prompt engineering, prompt, system prompt, instruction, context, AI interaction, improve results
  role: standard
  scope: productivity
  output-format: reference
  related-skills: context-management, skill-authoring, opencode-skill-creation
---

# Prompt Engineering

Library of proven prompt engineering patterns for optimal LLM results.

## Core Principles

1. **Start general, then specific** — Broad context first, then specific requirements
2. **Give examples** — Show input/output pairs the model can pattern-match
3. **Break complex tasks into simpler tasks** — One step at a time for complex work
4. **Avoid ambiguity** — Be explicit about what "this" refers to
5. **Indicate relative importance** — Flag what matters most in the request

## Prompt Patterns

### Zero-Shot Pattern
```
Write a [artifact] that [does X].
Requirements:
- [requirement 1]
- [requirement 2]
```

### Few-Shot Pattern
```
Generate [output type]. Examples:
Input: [example 1 input]
Output: [example 1 output]
Input: [example 2 input]
Output: [example 2 output]
Now process: [actual input]
```

### Chain-of-Thought Pattern
```
Work through this step by step:
1. First, [analysis step 1]
2. Then, [analysis step 2]
3. Finally, [conclusion]
```

### Structured Output Pattern
```
Return your answer as JSON with this schema:
{
  "field1": "<description>",
  "field2": "<description>"
}
Data to process: [input]
```

### Role Pattern
```
You are a [role] with expertise in [domain].
Your task is to [describe task].
Follow these rules:
- [rule 1]
- [rule 2]
```

### Constraint Pattern
```
[Task description]
Constraints:
- [hard constraint 1]
- [hard constraint 2]
Preferences:
- [soft preference 1]
```

### Persona Pattern
```
Act as a [specific persona] reviewing/creating/analyzing [artifact].
Your perspective is [describe perspective].
```

## Techniques for Coding Agents

### Context Budgeting
- Put the most important instructions first (primacy effect)
- Group related rules under clear headings
- Use hierarchical structure for easy scanning
- Remove redundant or contradictory instructions

### Instruction Layering
```
Layer 1: Role and goal (who the agent is, what to accomplish)
Layer 2: Always-on rules (hard constraints, non-negotiable)
Layer 3: Conditional rules (apply based on context)
Layer 4: Output formatting (how to present results)
Layer 5: Examples (concrete demonstrations)
```

### Avoiding Common Pitfalls
| Pitfall | Problem | Fix |
|---------|---------|-----|
| Vague instructions | Model guesses wrong | Be specific, measurable |
| Contradictory rules | Model picks randomly | Resolve conflicts explicitly |
| Over-constrained | Model can't satisfy all rules | Prioritize, distinguish hard vs soft |
| Hidden assumptions | Model doesn't know context | State explicit context |
| No error handling | Model fails silently | Define fallback behavior |

## Task Decomposition

For complex tasks, decompose into sub-tasks:
1. Analysis — Understand the problem and requirements
2. Planning — Determine approach and architecture
3. Implementation — Write code incrementally
4. Verification — Test and validate
5. Review — Self-review and fix issues
