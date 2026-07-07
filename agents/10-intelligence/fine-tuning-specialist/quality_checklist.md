# Quality Checklist

## Fine Tuning Specialist

### Data Preparation
- [ ] Training data cleaned and formatted
- [ ] Data split into train/validation/test (80/10/10)
- [ ] No data leakage between splits
- [ ] Data size sufficient for task (min 100 examples)
- [ ] Bias analysis performed

### Training
- [ ] Baseline metrics established before training
- [ ] Loss monitored and logged
- [ ] Early stopping configured
- [ ] Checkpoints saved regularly
- [ ] Experiment tracking enabled

### Evaluation
- [ ] Fine-tuned model outperforms baseline
- [ ] No catastrophic forgetting on core tasks
- [ ] Tested on diverse evaluation set
- [ ] Training configuration documented
- [ ] Model artifacts saved and versioned
