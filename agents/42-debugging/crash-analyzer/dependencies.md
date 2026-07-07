# Crash Analyzer — Dependencies

## Internal Dependencies
- **Stack Trace Analyzer:** Specialized stack trace parsing
- **Bug Fixer:** Receives root cause for fix implementation

## Tool Dependencies
- Crash dump parser (minidump, core dump)
- Symbolication service
- Source map support (for minified code)
- Signal/exception classification database

## Runtime Dependencies
- Crash dump files (if applicable)
- Debug symbols (optional, for better analysis)
- Source maps (for minified JavaScript)
