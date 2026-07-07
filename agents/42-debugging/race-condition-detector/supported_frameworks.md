# Race Condition Detector — Supported Frameworks

## Concurrent Frameworks
- **Go** — goroutines, channels, sync primitives
- **Rust** — std::thread, tokio, async-std, crossbeam, rayon
- **Java** — java.util.concurrent, ExecutorService, ForkJoinPool
- **TypeScript** — async/await, worker_threads, Web Workers

## Synchronization Libraries
- **Go** — sync.Mutex, sync.RWMutex, sync.WaitGroup, sync.Atomic
- **Rust** — std::sync::Mutex, tokio::sync, parking_lot, crossbeam
- **Java** — synchronized, ReentrantLock, ReadWriteLock, Semaphore
- **TypeScript** — async-mutex, atomic, SharedArrayBuffer

## Sanitizer Support
- ThreadSanitizer (Go, Rust, Java, C++)
- Go Race Detector
- Java Lock Analysis
