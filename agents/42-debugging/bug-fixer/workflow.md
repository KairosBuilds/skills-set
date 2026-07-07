# Bug Fixer — Workflow

1. **Input Reception**
   - Bug report with location (file, line) and description
   - Optional: expected behavior, reproduction steps

2. **Root Cause Analysis**
   - Read and understand the affected code
   - Trace execution path to confirm the bug
   - Identify all paths affected by the fix

3. **Fix Design**
   - Determine minimal change to address root cause
   - Consider alternative approaches
   - Ensure fix preserves existing behavior for non-bug paths

4. **Backup & Apply**
   - Create backup of original file
   - Apply minimal fix with inline comments explaining the change
   - Update associated tests or add new ones

5. **Verification**
   - Verify code compiles without errors
   - Run existing test suite
   - Run new tests for the fix
   - Check for side effects

6. **Output**
   - Provide diff of changes
   - Explain the fix rationale
   - Confirm test results
