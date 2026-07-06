# Stack Trace Analyzer — Limitations

## Parsing Limitations
- Corrupted stack traces may be unparseable
- Optimized code may have missing or incorrect frame information
- Inlined functions may not appear in stack traces
- Tail-call optimized frames may be missing

## Analysis Limitations
- Cannot determine root cause from stack trace alone for memory corruption
- Async stack traces may have incomplete continuation chains
- Minified JavaScript without source maps cannot be accurately mapped
- Mixed-language stacks (Java native, Python C extension) are harder to analyze

## Platform Limitations
- Release builds without debug symbols have limited frame information
- JIT-compiled code may have incomplete stack metadata
- Some platforms truncate deep stack traces
- Signal handler stacks may not capture the full call path
