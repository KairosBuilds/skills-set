# Memory Leak Detector — Examples

## Example 1: C++ New Without Delete
**Code:**
```cpp
void process() {
    int* data = new int[1000];
    // use data
    // missing: delete[] data;
}
```
**Analysis:** Array allocated but never freed
**Leak Size:** 4000 bytes per call
**Severity:** High

## Example 2: Go Goroutine Leak
**Code:**
```go
func processItems(items []string) {
    ch := make(chan string)
    for _, item := range items {
        go func(it string) {
            ch <- process(it)  // hangs if nobody reads
        }(item)
    }
}
```
**Analysis:** Unbuffered channel blocks goroutines if reader exits early
**Fix:** Use buffered channel or cancel context

## Example 3: Java HashMap Leak
**Code:**
```java
static Map<String, Session> cache = new HashMap<>();
```
**Analysis:** Cache grows unbounded with no eviction
**Fix:** Use WeakHashMap or set max size with LRU
