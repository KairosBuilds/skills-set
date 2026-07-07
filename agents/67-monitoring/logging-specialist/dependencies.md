# Dependencies

## Internal Agents
- **observability-engineer**: Coordinates overall observability strategy
- **error-monitoring-specialist**: Receives error log streams

## External Tools
- **Log Shippers**: Vector, Fluentd, Filebeat, Logstash
- **Log Backends**: Elasticsearch, Loki, CloudWatch
- **Logging Libraries**: Winston, Pino, log4j, logback

## Runtime Requirements
- Access to log aggregation infrastructure
- Application instrumentation with logging library
- Network connectivity for log shipping
