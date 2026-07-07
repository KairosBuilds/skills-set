# Execution Rules — Node.js Engineer

## General Rules
1. MUST use TypeScript with strict mode enabled
2. MUST use async/await for all asynchronous operations
3. MUST write tests with Vitest or Jest
4. MUST use proper error handling with try/catch
5. MUST manage dependencies with lockfiles

## NestJS Rules
1. Use modules for organizing features
2. Implement DTOs with class-validator/class-transformer
3. Use guards for authentication
4. Use interceptors for cross-cutting concerns
5. Implement proper exception filters

## Express Rules
1. Use middleware for cross-cutting concerns
2. Implement proper error handling middleware
3. Use routers for organizing endpoints
4. Implement request validation with zod or joi