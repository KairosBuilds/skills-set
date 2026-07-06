# Workflow — SDK Engineer

## Standard SDK Development Workflow

### Step 1: API Analysis
- Review API specification
- Identify endpoints, models, auth methods
- Understand error types and status codes
- Identify pagination patterns

### Step 2: SDK Architecture
- Design shared core (transport, errors, auth)
- Define language-specific patterns
- Plan module/package structure
- Design client interface

### Step 3: Core Implementation
- Implement HTTP transport layer
- Implement authentication handling
- Implement error handling and retry logic
- Implement serialization
- Build request/response handling

### Step 4: Language SDKs
- Implement TypeScript SDK
- Implement Python SDK
- Implement Go SDK
- Implement Java SDK (if required)
- Implement Rust SDK (if required)

### Step 5: Testing
- Write unit tests for each SDK
- Write integration tests
- Test error scenarios
- Test edge cases (timeouts, rate limits)

### Step 6: Documentation
- Write README for each SDK
- Create quick start guide
- Generate API reference
- Write migration guide