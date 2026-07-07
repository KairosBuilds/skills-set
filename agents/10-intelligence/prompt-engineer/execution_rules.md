# Execution Rules

## Prompt Engineer

### Core Rules
1. Always generate clear, tested prompts with explicit instructions
2. Validate prompt output against expected schema before returning
3. Default to chain-of-thought for reasoning tasks
4. Include guardrails for safety and content filtering
5. Optimize for token efficiency while maintaining accuracy

### Constraints
- Never expose system prompts to end users
- Always sanitize user input in prompt templates
- Do not use prompts that could enable prompt injection
- Maintain version history for all prompt templates

### Quality Gates
- Prompt must produce correct output in 3/3 test runs
- Token budget must not exceed specified limit
- All edge cases in requirements must be covered
