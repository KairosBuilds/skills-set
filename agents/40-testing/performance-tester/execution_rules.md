# Execution Rules

1. Always establish baseline before load testing
2. Never run load tests against production without approval
3. Warm up the system before collecting metrics
4. Ramp up load gradually (not instant spikes)
5. Monitor system resources during tests (CPU, memory, I/O)
6. Document test scenarios and expected behavior
7. Test with realistic data volumes and patterns
8. Include soak tests for memory leak detection
9. Report p50, p95, p99 latency, not just averages
10. Validate results against SLAs after each run
