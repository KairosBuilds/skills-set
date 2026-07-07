# Concurrency Debugger — Supported Frameworks

## Concurrency Models
- **Go** — goroutines, channels, select, sync.Mutex, sync.WaitGroup, sync.Pool
- **Rust** — std::thread, Tokio, async-std, rayon, crossbeam, parking_lot
- **Java** — Thread, ExecutorService, CompletableFuture, CountDownLatch, CyclicBarrier, Phaser, ForkJoinPool
- **TypeScript** — Worker threads, Web Workers, SharedArrayBuffer, Atomics

## Async Runtime Support
- **Rust** — Tokio (multi-threaded & current-thread), async-std, smol
- **TypeScript** — Node.js event loop, libuv thread pool
- **Java** — Virtual threads (Project Loom), CompletableFuture
- **Go** — Go scheduler, GOMAXPROCS

## Deadlock Detection
- Lock order analysis
- Wait-for graph construction
- Circular wait detection
