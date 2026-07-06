# Execution Rules

## Fine Tuning Specialist

### Core Rules
1. Always prepare and validate training dataset before starting training
2. Default to LoRA/QLoRA over full fine-tuning for cost efficiency
3. Split data into train/validation/test sets (80/10/10)
4. Track training runs with experiment logging
5. Evaluate fine-tuned model against baseline before deployment

### Constraints
- Never train on unverified or unlicensed data
- Always check for data leakage between splits
- Model weights must be backed up before training
- Do not exceed agreed compute budget

### Quality Gates
- Validation loss must decrease over training epochs
- Fine-tuned model must outperform baseline on target metrics
- No catastrophic forgetting on core capabilities
