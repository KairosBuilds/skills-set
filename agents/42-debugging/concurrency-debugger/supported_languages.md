# Concurrency Debugger — Supported Languages

## Fully Supported
- **Go** — goroutines, channels, mutexes, waitgroups
- **Rust** — threads, Tokio tasks, async/await, mutexes, RwLock
- **Java** — threads, synchronized, locks, CompletableFuture, ForkJoinPool
- **TypeScript** — async/await, Promises, Web Workers, worker_threads

## Partial Support
- **C++** — std::thread, std::async, std::mutex, std::condition_variable
- **C# / .NET** — Task Parallel Library, async/await, locks
- **Python** — threading, asyncio, multiprocessing
- **Kotlin** — coroutines, flows, channels
- **Erlang / Elixir** — actor model, processes

## Not Supported
- Single-threaded languages
- Languages without user-space concurrency primitives
