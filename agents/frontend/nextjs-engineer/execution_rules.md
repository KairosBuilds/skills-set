# Execution Rules for Next.js Engineer Agent

## Core Rules

1. **App Router Only**: Use App Router (`app/` directory). Never use Pages Router unless explicitly requested for legacy projects.
2. **Server Components First**: All components are Server Components by default. Use `'use client'` only when interactivity, hooks, or browser APIs are needed.
3. **Data Fetching**: Prefer server-side data fetching in Server Components. Use `fetch()` with caching options, not `useEffect` for data loading.
4. **Server Actions**: Use Server Actions for form submissions and mutations. Validate with Zod on both client and server.
5. **SEO**: Every page must export `generateMetadata()` for dynamic metadata. Use appropriate meta tags and structured data.
6. **Performance**: Use `next/image` for images, `next/link` for client-side navigation, `next/font` for fonts.
7. **Streaming**: Use `loading.tsx` and `Suspense` boundaries for streaming progressive rendering.
8. **Error Handling**: Use `error.tsx` boundaries at every route segment. Provide meaningful error UI.
9. **Route Groups**: Use route groups `(groupName)` for layout organization without affecting URL structure.
10. **Middleware**: Use middleware for auth, redirects, and internationalization sparingly.

## Prohibited

- `getServerSideProps`, `getStaticProps`, `getInitialProps` (Pages Router legacy)
- `_app.tsx`, `_document.tsx` overrides unless strictly necessary
- Client-side data fetching without Suspense
- Inline `<img>` tags without optimization
- Direct `window`/`document` reference in Server Components
- `useEffect` for data fetching

## Enforcement

Run `npm run build` (which includes type checking and linting) before completing.
