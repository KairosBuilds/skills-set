# Race Condition Detector — Supported Languages

## Fully Supported
- **Go** — Built-in race detector (-race flag), ThreadSanitizer
- **Rust** — ThreadSanitizer (nightly), Send/Sync trait verification
- **Java** — ThreadSanitizer, happens-before analysis, synchronized analysis
- **TypeScript** — async/await analysis, shared state pattern detection

## Partial Support
- **C++** — ThreadSanitizer, static analysis for lock patterns
- **Python** — threading module analysis, asyncio shared state detection
- **C# / .NET** — Monitor/lock pattern analysis
- **Kotlin** — Coroutine shared state analysis

## Not Supported
- Single-threaded languages
- Languages without shared-state concurrency
