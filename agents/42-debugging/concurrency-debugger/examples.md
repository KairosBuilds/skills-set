# Concurrency Debugger — Examples

## Example 1: Deadlock with Mutex (Go)
**Code:**
```go
func transfer(from, to *Account, amount int) {
    from.mu.Lock()
    to.mu.Lock()    // deadlock if two transfers happen in opposite order
    from.balance -= amount
    to.balance += amount
    to.mu.Unlock()
    from.mu.Unlock()
}
```
**Analysis:** Lock ordering inversion causes circular wait
**Fix:** Always acquire locks in consistent global order or use trylock

## Example 2: Orphaned Goroutine (Go)
**Code:**
```go
go func() {
    result := await slowOperation()
    ch <- result
}()
// main path returns early, nobody reads ch
```
**Analysis:** Goroutine blocks forever writing to unbuffered channel
**Fix:** Use context cancellation and buffered channel

## Example 3: Thread Starvation (Java)
**Code:**
```java
synchronized (bigLock) {
    // long-running operation holding lock
    // other threads waiting for bigLock starve
}
```
**Analysis:** Coarse-grained locking causes thread starvation
**Fix:** Use fine-grained locks or read-write locks
