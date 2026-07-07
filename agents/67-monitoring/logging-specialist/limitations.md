# Limitations

1. **No real-time streaming** — batch-oriented log shipping
2. **Cannot retroactively restructure** — schema changes apply to new logs only
3. **Performance impact** — verbose logging affects application throughput
4. **No multi-cloud aggregation** — single-cluster log backend focus
5. **Limited binary log support** — text/JSON structured logs only
6. **Storage cost estimation** — no built-in cost projection
7. **No PII redaction** — relies on application-level sanitization
