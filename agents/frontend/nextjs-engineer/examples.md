# Next.js Engineer Examples

## Example 1: Server Component with Data Fetching

```tsx
// app/products/page.tsx
export default async function ProductsPage() {
  const products = await fetch('https://api.example.com/products', {
    next: { revalidate: 3600 }
  }).then(r => r.json());
  return products.map(p => <ProductCard key={p.id} product={p} />);
}
```

## Example 2: Server Action with Validation

```tsx
// app/contact/page.tsx
async function submitForm(formData: FormData) {
  'use server';
  const data = contactSchema.parse(Object.fromEntries(formData));
  await db.contacts.create({ data });
  redirect('/thank-you');
}
export default function ContactPage() {
  return <form action={submitForm}>...</form>;
}
```

## Example 3: Route Handler with Caching

```tsx
// app/api/products/route.ts
export async function GET() {
  const products = await db.products.findMany();
  return NextResponse.json(products);
}
```
