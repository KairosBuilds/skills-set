# Bug Fixer — Examples

## Example 1: Fix Null Pointer Dereference
**Before:**
```javascript
function processUser(user) {
  return user.name.toUpperCase();
}
```
**After:**
```javascript
function processUser(user) {
  if (!user) return '';
  return user.name.toUpperCase();
}
```
**Tests added:** null input, undefined input, valid user

## Example 2: Fix SQL Injection
**Before:**
```javascript
query = "SELECT * FROM users WHERE id = " + userId;
```
**After:**
```javascript
query = "SELECT * FROM users WHERE id = $1";
// Using parameterized query
```
**Tests added:** SQL injection attempt, valid ID

## Example 3: Fix Off-by-One
**Before:**
```java
for (int i = 0; i <= array.length; i++) { ... }
```
**After:**
```java
for (int i = 0; i < array.length; i++) { ... }
```
**Tests added:** empty array, single element, full array
