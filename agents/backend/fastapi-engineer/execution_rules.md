# Execution Rules — FastAPI Engineer

## General Rules
1. MUST use async endpoints for I/O operations
2. MUST use Pydantic v2 models for validation
3. MUST use dependency injection for shared logic
4. MUST write pytest tests with HTTPX async client
5. MUST generate OpenAPI documentation

## Design Rules
1. Use Pydantic models for request/response schemas
2. Implement proper HTTP exception handlers
3. Use background tasks for non-critical operations
4. Implement proper CORS configuration
5. Use lifespan events for startup/shutdown

## Performance Rules
1. Use async database drivers (asyncpg, aiomysql)
2. Use connection pooling for database
3. Implement caching with Redis
4. Use streaming responses for large payloads
5. Configure gunicorn/uvicorn for production