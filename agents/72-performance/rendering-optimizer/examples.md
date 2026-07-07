# Examples

## React Profiler
```typescript
import { Profiler } from 'react';

function onRender(id, phase, actualDuration) {
  console.log(`${id} ${phase}: ${actualDuration}ms`);
}

<Profiler id="Dashboard" onRender={onRender}>
  <Dashboard />
</Profiler>
```

## Prevent Wasted Renders
```typescript
const ExpensiveList = React.memo(({ items }) => (
  <ul>{items.map(item => <li key={item.id}>{item.name}</li>)}</ul>
));
```
