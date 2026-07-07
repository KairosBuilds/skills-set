# Workflow

1. Identify component boundaries and integration points
2. Set up Docker containers for dependencies (DBs, message queues, caches)
3. Configure test data and schema migrations
4. Write integration tests covering:
   - Database read/write operations
   - API endpoint contracts
   - Message queue produce/consume cycles
   - Service-to-service communication
5. Execute tests against real containers
6. Validate error handling across boundaries
7. Test transaction rollback scenarios
8. Verify idempotency and retry behavior
