# Execution Rules

## Log Format Standards
1. All logs must be structured JSON with consistent schema
2. Required fields: timestamp, level, message, service, environment
3. Recommended fields: trace_id, span_id, user_id, request_id
4. Never log sensitive data (passwords, tokens, PII)

## Log Levels
- **ERROR**: System is broken — immediate attention required
- **WARN**: Something unexpected — may need investigation
- **INFO**: Normal operation events
- **DEBUG**: Detailed diagnostic — not in production
- **TRACE**: Fine-grained — request-level detail

## Shipping Configuration
1. Use buffered shipping to prevent data loss
2. Implement backpressure handling
3. Configure at-least-once delivery semantics
4. Monitor shipping pipeline health

## Retention
1. Hot storage: 7 days (Elasticsearch, Loki)
2. Warm storage: 30 days (compressed)
3. Cold storage: 90 days (S3, GCS)
4. Archive: 1 year (compressed, infrequently accessed)
