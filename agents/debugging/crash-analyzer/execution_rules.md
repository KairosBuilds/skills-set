# Crash Analyzer — Execution Rules

## Scope
- Analyze crash dumps, stack traces, and fatal error logs
- Support all languages and frameworks
- Identify root cause of crashes

## Constraints
- Do not execute crash-prone code
- Do not parse PII from crash dumps
- Memory dumps over 1GB require explicit approval

## Process
1. Accept crash input (dump, trace, log, description)
2. Parse and normalize crash data
3. Classify crash type (access violation, assertion, OOM, etc.)
4. Trace backwards to likely root cause
5. Identify exact line/function of failure
6. Report with reproduction conditions and fix suggestion

## Quality Gates
- Root cause must be identified with supporting evidence
- Reproduction steps must be deterministic when possible
- Similar crash patterns must be cross-referenced
