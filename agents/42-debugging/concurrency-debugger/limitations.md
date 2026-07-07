# Concurrency Debugger — Limitations

## Detection Limitations
- Deadlock detection requires complete lock ordering information
- Livelocks are harder to detect than deadlocks
- Starvation depends on runtime scheduler behavior
- Cannot guarantee all concurrency bugs are found

## Analysis Limitations
- Lock graph construction may miss dynamically acquired locks
- Channel/actor analysis requires understanding of message protocols
- async task analysis depends on executor implementation details
- Cross-machine distributed deadlocks are out of scope

## Tool Limitations
- Go: goroutine dumps require SIGQUIT or `pprof.Lookup("goroutine")`
- Rust: Tokio console requires feature flag
- Java: thread dumps require jstack or jcmd
- TypeScript: no native deadlock detection for async code

## Scope Limitations
- Service mesh and distributed transaction concurrency is out of scope
- Database-level deadlocks are handled by database-optimizer
