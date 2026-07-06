# Race Condition Detector — Examples

## Example 1: Shared Counter Without Mutex (Go)
**Code:**
```go
var counter int
for i := 0; i < 1000; i++ {
    go func() { counter++ }()  // data race
}
```
**Analysis:** Multiple goroutines write to counter without synchronization
**Fix:** Use `sync.Mutex` or `atomic.AddInt64`

## Example 2: Check-Then-Act (Java)
**Code:**
```java
if (!map.containsKey(key)) {
    map.put(key, value);  // race: another thread may have put already
}
```
**Analysis:** Non-atomic check-then-act pattern
**Fix:** Use `computeIfAbsent` or synchronized block

## Example 3: Double-Checked Locking (C++)
**Code:**
```cpp
if (!instance) {           // read without lock
    lock_guard lock(mtx);
    if (!instance) {
        instance = new T();  // race: write without full barrier
    }
}
```
**Analysis:** Missing memory barrier on read
**Fix:** Use `std::atomic` with acquire-release semantics
