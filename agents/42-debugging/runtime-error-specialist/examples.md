# Runtime Error Specialist — Examples

## Example 1: NullPointerException (Java)
**Input:**
```java
String name = getUser().getName(); // getUser() returns null
```
**Analysis:** `getUser()` returns null when user not found
**Fix:** Add null check before method call

## Example 2: TypeError (Python)
**Input:**
```python
result = 10 + "5"  # TypeError: unsupported operand type
```
**Analysis:** Mixing int and str without conversion
**Fix:** Ensure type consistency or explicit conversion

## Example 3: IndexError (Python)
**Input:**
```python
items = []
first = items[0]  # IndexError: list index out of range
```
**Analysis:** Empty list access without check
**Fix:** Check list length before accessing
