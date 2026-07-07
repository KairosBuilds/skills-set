# Examples

## Optimization: Nested Loop → Hash Map
```typescript
// Before: O(n*m)
function findDuplicates(listA: number[], listB: number[]) {
  return listA.filter(a => listB.includes(a));
}

// After: O(n+m)
function findDuplicates(listA: number[], listB: number[]) {
  const setB = new Set(listB);
  return listA.filter(a => setB.has(a));
}
```

## Optimization: Recursion → Iteration
```typescript
// Before: O(n) stack space
function factorial(n: number): number {
  return n <= 1 ? 1 : n * factorial(n - 1);
}

// After: O(1) stack space
function factorial(n: number): number {
  let result = 1;
  for (let i = 2; i <= n; i++) result *= i;
  return result;
}
```
