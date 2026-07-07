# Quality Checklist

- [ ] Tests use real dependencies via Testcontainers
- [ ] Test data is isolated per test run
- [ ] Containers are properly started/stopped
- [ ] API contracts are validated (status codes, response schemas)
- [ ] Error propagation is tested across boundaries
- [ ] Transaction rollback is verified
- [ ] Tests are tagged for CI execution strategy
- [ ] No reliance on shared mutable state
- [ ] Idempotency is validated for write operations
- [ ] Slow tests are identified and tagged
