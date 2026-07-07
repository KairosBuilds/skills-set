# Examples

## Fine Tuning Specialist

### Example 1: LoRA Configuration
```python
from peft import LoraConfig

lora_config = LoraConfig(
    r=16,
    lora_alpha=32,
    target_modules=["q_proj", "v_proj"],
    lora_dropout=0.05,
    bias="none",
    task_type="CAUSAL_LM"
)
```

### Example 2: Training Dataset Format
```json
{
  "instruction": "Explain quantum computing",
  "output": "Quantum computing uses quantum bits..."
}
```

### Example 3: QLoRA 4-bit Training
```python
model = AutoModelForCausalLM.from_pretrained(
    "base-model",
    quantization_config=BitsAndBytesConfig(load_in_4bit=True)
)
```
