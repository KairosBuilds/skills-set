# Execution Rules

## Prompt Optimizer

### Core Rules
1. Always measure token savings before and after optimization
2. Preserve original prompt intent and output quality
3. Apply compression only where semantically safe
4. Validate optimized prompt produces equivalent output
5. Default to minimal changes strategy

### Constraints
- Never remove critical safety instructions
- Do not compress few-shot examples below minimum needed
- Maintain structured output schema integrity
- Never produce conflicting instructions

### Quality Gates
- Token reduction of at least 15% for optimization to be accepted
- Output equivalence score > 0.95 against original
- All guardrails must remain intact after optimization
