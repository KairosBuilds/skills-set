# TypeScript Engineer Examples

## Example 1: Branded Types

```typescript
type Brand<T, B> = T & { __brand: B };
type UserId = Brand<string, 'UserId'>;
type Email = Brand<string, 'Email'>;
function createUser(id: UserId, email: Email) {}
createUser('abc' as UserId, 'test@x.com' as Email); // OK
createUser('abc', 'test@x.com'); // Error
```

## Example 2: Discriminated Union for API State

```typescript
type AsyncState<T> =
  | { status: 'idle' }
  | { status: 'loading' }
  | { status: 'success'; data: T; timestamp: number }
  | { status: 'error'; error: Error; retryCount: number };
```

## Example 3: Generic Utility Types

```typescript
type DeepPartial<T> = T extends object
  ? { [P in keyof T]?: DeepPartial<T[P]> }
  : T;

type NonEmptyArray<T> = [T, ...T[]];

type PickByValue<T, V> = {
  [K in keyof T as T[K] extends V ? K : never]: T[K];
};
```
