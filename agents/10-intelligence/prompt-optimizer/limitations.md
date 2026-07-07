# Limitations

## Prompt Optimizer

### Known Limitations
1. Aggressive compression may reduce output quality
2. Not all verbose patterns can be safely optimized
3. Language-specific optimizations may not transfer across models
4. Cannot optimize beyond the semantic constraints of the task

### Mitigations
- Always validate optimized prompts against original
- Maintain minimum quality thresholds
- Support rollback to original prompt
- Test across multiple model versions
