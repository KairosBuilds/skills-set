# Bug Finder — Examples

## Example 1: Null Pointer Dereference
**Input:** JavaScript function without null check
```
function processUser(user) {
  return user.name.toUpperCase();
}
```
**Finding:** Null pointer risk — `user` could be undefined
**Severity:** Critical | **Confidence:** 95%

## Example 2: SQL Injection
**Input:** Raw string concatenation in SQL query
```
query = "SELECT * FROM users WHERE id = " + userId;
```
**Finding:** SQL injection vulnerability
**Severity:** Critical | **Confidence:** 99%

## Example 3: Off-by-One Loop
**Input:** Loop with incorrect boundary
```
for (int i = 0; i <= array.length; i++) { ... }
```
**Finding:** Array index out of bounds on last iteration
**Severity:** High | **Confidence:** 100%
