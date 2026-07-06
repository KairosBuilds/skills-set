# Execution Rules — C# Engineer

## General Rules
1. MUST use nullable reference types
2. MUST use async/await for I/O operations
3. MUST use dependency injection
4. MUST write xUnit tests with Moq/FluentAssertions
5. MUST use .NET 8+ features

## ASP.NET Core Rules
1. Use minimal or controller-based APIs appropriately
2. Implement proper middleware pipeline
3. Use options pattern for configuration
4. Implement proper exception handling middleware
5. Use structured logging (Serilog)

## EF Core Rules
1. Use migrations for schema changes
2. Use AsNoTracking for read-only queries
3. Use Include/ThenInclude for eager loading
4. Implement proper transaction management
5. Use query splitting for complex queries