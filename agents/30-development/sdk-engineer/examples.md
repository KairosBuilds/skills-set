# Examples — SDK Engineer

## Example: Payments API SDK
**Specification:** REST API for payment processing

**Languages:** TypeScript, Python, Go

**Implementation:**
1. Core: HTTP client, retry logic, auth handling
2. TypeScript: class-based client with full types
3. Python: client with context managers and type hints
4. Go: client struct with method receivers
5. Consistent patterns: PaymentClient.create(), .retrieve(), .list()
6. Automatic retry on 429 and 5xx errors
7. Rate limiting with configurable limits

**Output:** Multi-language SDK published to npm, PyPI, and GitHub