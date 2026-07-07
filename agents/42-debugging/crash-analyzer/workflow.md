# Crash Analyzer — Workflow

1. **Input Reception**
   - Crash dump, stack trace, core dump, or error log
   - Optional: application version, environment details

2. **Parse & Normalize**
   - Parse crash data into structured format
   - Normalize across different crash formats
   - Extract signal, exception type, faulting address

3. **Classify Crash Type**
   - Access violation / segfault
   - Null pointer dereference
   - Stack overflow / buffer overflow
   - Assertion failure
   - Out of memory
   - Unhandled exception
   - Corrupted state

4. **Root Cause Tracing**
   - Walk stack frames from crash point backwards
   - Identify first frame with application code
   - Determine the exact operation that failed

5. **Context Reconstruction**
   - Analyze variable states at crash point
   - Determine input or condition leading to crash
   - Check for similar crash patterns

6. **Report**
   - Crash type and classification
   - Root cause with file and line
   - Reproduction conditions
   - Fix recommendation
