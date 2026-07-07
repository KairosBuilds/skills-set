# Stack Trace Analyzer — Workflow

1. **Input Reception**
   - Raw stack trace text from any language
   - Optional: source maps, symbol files

2. **Parse & Normalize**
   - Detect stack trace format (Java, .NET, JS, Python, Go, Rust, C++, etc.)
   - Split into individual frames
   - Normalize to common frame format

3. **Frame Classification**
   - Application code (relevant)
   - Library/framework code (context)
   - Native frames (C/C++ in managed runtimes)
   - Internal runtime frames (usually irrelevant)

4. **Root Cause Identification**
   - Find first application frame in trace
   - For chained exceptions, unwrap to root cause
   - For async traces, correlate across continuation boundaries
   - Identify exact line and function of failure

5. **Source Mapping**
   - Map stack frame locations to source code
   - For minified JS, use source maps
   - For native code, use debug symbols if available

6. **Report**
   - Annotated stack trace with source context
   - Root cause classification
   - Relevant code snippets
   - Fix direction
