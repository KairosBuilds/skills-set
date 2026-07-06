# React Engineer Examples

## Example 1: Server Component with Data Fetching

```tsx
// app/products/page.tsx
async function ProductsPage() {
  const products = await fetchProducts();
  return (
    <div className="grid grid-cols-3 gap-4">
      {products.map((p) => <ProductCard key={p.id} product={p} />)}
    </div>
  );
}
```

## Example 2: Client Component with Optimistic Updates

```tsx
'use client';
function LikeButton({ postId }: { postId: string }) {
  const [liked, setLiked] = useState(false);
  const handleClick = async () => {
    setLiked(true);
    try { await api.like(postId); }
    catch { setLiked(false); }
  };
  return <button onClick={handleClick}>{liked ? '♥' : '♡'}</button>;
}
```

## Example 3: Compound Component Pattern

```tsx
<Select value={selected} onChange={setSelected}>
  <Select.Trigger>{selected.label}</Select.Trigger>
  <Select.Options>
    <Select.Option value="a">Option A</Select.Option>
    <Select.Option value="b">Option B</Select.Option>
  </Select.Options>
</Select>
```
