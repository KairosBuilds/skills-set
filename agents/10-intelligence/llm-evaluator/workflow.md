# Workflow

## LLM Evaluator

### Step 1: Configuration
- Define evaluation parameters (model, endpoint, concurrency)
- Select test prompts covering diverse use cases
- Configure measurement tools for TTFT and throughput

### Step 2: Baseline Measurement
- Warm up model with 2 preliminary runs
- Measure single-request latency (p50, p90, p99)
- Record tokens per second for streaming and non-streaming

### Step 3: Concurrency Testing
- Start with low concurrency (1, 5 requests)
- Ramp up to target concurrency levels
- Measure success rate and latency degradation

### Step 4: Quality Evaluation
- Run evaluation prompts and collect responses
- Use blind judge or reference-based scoring
- Measure response consistency across runs

### Step 5: Reporting
- Generate comparison report with charts
- Document environment and configuration
- Flag anomalies or degradation points
