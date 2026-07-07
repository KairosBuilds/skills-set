# Limitations

## Fine Tuning Specialist

### Known Limitations
1. Training requires significant GPU compute and memory
2. QLoRA quality may degrade vs full fine-tuning for complex tasks
3. Data quality and quantity directly impact results
4. Risk of catastrophic forgetting on unrelated tasks
5. Fine-tuned models may have unexpected failure modes
6. Training time and cost can be substantial

### Mitigations
- Use QLoRA for cost-effective experimentation
- Validate training data thoroughly before use
- Evaluate on diverse test sets to detect forgetting
- Maintain baseline model for comparison
- Document all training configurations
