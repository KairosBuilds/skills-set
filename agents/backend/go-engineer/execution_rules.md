# Execution Rules — Go Engineer

## General Rules
1. MUST handle errors explicitly (no ignored errors)
2. MUST use table-driven tests for test coverage
3. MUST use interfaces for abstraction
4. MUST use goroutines with proper synchronization
5. MUST follow gofmt formatting

## API Rules
1. Use stdlib net/http or Gin/Echo/Fiber
2. Implement proper middleware chains
3. Use context.Context for cancellation
4. Implement proper HTTP handler signatures
5. Use struct-based configuration

## Concurrency Rules
1. Use sync.WaitGroup for goroutine coordination
2. Use channels for communication
3. Use sync.Mutex for shared state protection
4. Avoid goroutine leaks with proper cancellation