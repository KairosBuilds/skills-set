# Limitations

## AI Workflow Designer

### Known Limitations
1. Complex workflows may hit LLM context window limits
2. Agent loops can accumulate errors across steps
3. Tool failures may not be gracefully handled by all LLMs
4. Debugging multi-step agent behavior is complex
5. Workflow latency increases with each sequential step

### Mitigations
- Implement checkpointing and logging at each step
- Set maximum iteration limits for all loops
- Include error handling and retry logic
- Test workflows in isolation before integration
- Monitor cost and latency per workflow execution
