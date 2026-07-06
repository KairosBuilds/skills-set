# Crash Analyzer — Limitations

## Data Limitations
- Requires readable crash dump or stack trace
- Cannot analyze crashes without debugging symbols or source maps
- Memory corruption crashes may have unreliable stack traces
- Optimized release builds may have incomplete frame information

## Scope Limitations
- Cannot reproduce crashes without reproduction steps
- Intermittent crashes may not leave sufficient evidence
- Cannot analyze kernel-level crashes without kernel debug symbols
- Distributed system crashes may require multiple correlated dumps

## Platform Limitations
- Core dump analysis requires matching binary and debug symbols
- MiniDump analysis requires Microsoft debugging tools
- Java heap dump analysis requires proper JVM flags
- iOS crash reports require symbolication with dSYM files
