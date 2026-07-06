# Examples

## Redis Cache-Aside (Node.js)
```typescript
async function getUser(id: string) {
  const cached = await redis.get(`user:${id}`);
  if (cached) return JSON.parse(cached);
  
  const user = await db.findUser(id);
  await redis.setex(`user:${id}`, 3600, JSON.stringify(user));
  return user;
}
```

## HTTP Cache Headers
```typescript
// Static assets — cache for 1 year
res.setHeader('Cache-Control', 'public, max-age=31536000, immutable');

// API responses — validate with ETag
res.setHeader('Cache-Control', 'no-cache');
res.setHeader('ETag', `"${hash}"`);
```
