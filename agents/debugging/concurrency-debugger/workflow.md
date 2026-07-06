# Concurrency Debugger — Workflow

1. **Input Reception**
   - Concurrent code (goroutines, threads, async tasks)
   - Or: execution trace, deadlock dump, hang report

2. **Task/Thread Map**
   - Identify all execution contexts (goroutines, threads, tasks)
   - Map creation and lifecycle
   - Determine synchronization points

3. **Lock Graph Construction**
   - Build directed graph of locks and ordering
   - Identify circular wait conditions (deadlock)
   - Detect single-thread bottlenecks (contention)

4. **Starvation Analysis**
   - Check scheduling fairness
   - Identify busy-waiting patterns
   - Detect priority inversion

5. **Channel/Actor Analysis**
   - Analyze channel send/receive patterns
   - Identify unbounded buffering
   - Detect actor mailbox overflow

6. **Report**
   - Deadlock cycle or contention point
   - Lock graph visualization
   - Fix recommendation with restructured code
