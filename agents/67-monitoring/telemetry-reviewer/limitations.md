# Limitations

1. **No auto-instrumentation** — reviews manual instrumentation only
2. **Cannot generate spans** — analysis-only, no runtime modification
3. **No profile data analysis** — CPU/memory profiling not covered
4. **Static analysis only** — does not run tests to verify telemetry output
5. **Limited to OpenTelemetry** — not compatible with proprietary tracing
6. **No real-time validation** — reviews code/config not live traffic
7. **Sample-based review** — may miss intermittent instrumentation gaps
