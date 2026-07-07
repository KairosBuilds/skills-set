# Runtime Error Specialist — Workflow

1. **Input Reception**
   - Exception type, message, stack trace
   - Input data that triggered the error
   - Optional: code context around the error

2. **Error Classification**
   - NullReference / NullPointerException
   - IndexOutOfBounds / RangeError
   - TypeError / ClassCastException
   - DivisionByZero / ArithmeticException
   - ResourceExhausted (file handles, sockets)
   - IllegalState / InvalidOperation

3. **State Tracing**
   - Trace backwards from error location
   - Identify how problematic state was created
   - Determine which check or validation is missing

4. **Input Analysis**
   - Analyze the input that triggered the error
   - Identify input characteristics that bypass safeguards
   - Generalize to input pattern

5. **Fix Strategy**
   - Add missing validation or null check
   - Implement defensive programming patterns
   - Use language-specific safety features
   - Add proper error handling

6. **Report**
   - Error type and location
   - Triggering input pattern
   - Root cause analysis
   - Fix with defensive pattern
