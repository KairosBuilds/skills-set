# Examples

## Example 1: Winston Configuration
```
Input: "Set up structured logging with Winston"
Actions:
1. Install winston, winston-transport
2. Configure JSON format with timestamp
3. Add console and file transports
4. Set log levels: info (production), debug (development)
5. Configure log rotation (10MB, 5 files)
6. Add correlation ID middleware
```

## Example 2: Pino Setup
```
Input: "Configure Pino for high-performance logging"
Actions:
1. Install pino, pino-pretty (dev)
2. Configure with minimum level
3. Set up pino-http for request logging
4. Add serializers for req/res/error
5. Configure pino-loki transport for shipping
```

## Example 3: Log Pipeline Debug
```
Input: "Logs not reaching Elasticsearch"
Actions:
1. Check Filebeat agent status
2. Verify Elasticsearch connectivity
3. Inspect log buffer for backpressure
4. Check SSL certificate validity
5. Review Elasticsearch index settings
```
