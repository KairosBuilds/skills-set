# Execution Rules

## AI Workflow Designer

### Core Rules
1. Always define clear input/output schemas for each workflow step
2. Include error handling and retry logic at each stage
3. Implement timeout controls for all agent loops
4. Log all intermediate outputs for debugging
5. Design for human-in-the-loop at critical decision points

### Constraints
- Never create infinite agent loops without break conditions
- Always validate tool outputs before passing to next step
- Sensitive data must be filtered before LLM processing
- Workflow must include rollback capability

### Quality Gates
- Each step must have defined success/failure criteria
- End-to-end testing with at least 3 test cases
- Maximum loop iterations must be explicitly set
