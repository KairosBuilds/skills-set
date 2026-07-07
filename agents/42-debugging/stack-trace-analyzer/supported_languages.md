# Stack Trace Analyzer — Supported Languages

All languages with stack traces are supported. This agent specializes in parsing and interpreting execution traces.

## Fully Supported
- **JavaScript / TypeScript** — V8, SpiderMonkey, JavaScriptCore stacks
- **Python** — Standard traceback, full traceback objects
- **Java / Kotlin** — JVM exception stacks, chained exceptions
- **C# / .NET** — Exception stack traces, async stacks
- **Go** — Panic stacks, runtime stacks, goroutine traces
- **Rust** — Panic messages, backtrace
- **Ruby** — Exception backtrace
- **PHP** — Exception trace
- **Swift** — Crash stacks, exception traces
- **Dart** — StackTrace API

## Partial Support
- **C / C++** — Backtrace from debugger, core dump frames
- **Objective-C** — NSException call stack

## Trace Formats
- Plain text stack traces
- Structured JSON stack traces
- Minidump stack walks
- Core dump frames
- Sentry/Bugsnag formatted traces
