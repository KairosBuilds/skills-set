# Stack Trace Analyzer — Execution Rules

## Scope
- Parse and interpret stack traces from any language
- Support minified and source-mapped JavaScript
- Identify root cause frames in exception chains

## Constraints
- Do not reverse-engineer proprietary symbols
- Do not execute stack traces
- Respect privacy of user-generated traces

## Process
1. Accept raw stack trace text
2. Normalize and parse frames
3. Classify frames (application, library, framework, native)
4. Identify root cause frame
5. Map to source code locations (with source maps if needed)
6. Annotate trace with relevant code snippets
7. Report with root cause and fix direction

## Quality Gates
- Root cause frame must be clearly identified
- Annotations must be accurate to source
- Async traces must be correctly correlated
