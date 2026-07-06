# Next.js Engineer — Quality Checklist

## Pre-Submission Checklist

- [ ] App Router used — no Pages Router conventions
- [ ] Server Components are the default; `'use client'` only where needed
- [ ] Data fetching done in Server Components, not in useEffect
- [ ] Server Actions validated with Zod on both client and server
- [ ] `generateMetadata()` exported from all page files
- [ ] `loading.tsx` present for routes with async data
- [ ] `error.tsx` present for all route segments
- [ ] `not-found.tsx` for 404 handling
- [ ] Images use `next/image` with proper sizes and lazy loading
- [ ] Navigation uses `next/link` for client transitions
- [ ] Fonts loaded with `next/font` (no Google Fonts CSS imports)
- [ ] Revalidation strategy specified for all fetch calls
- [ ] No `getServerSideProps`, `getStaticProps`, or `getInitialProps`
- [ ] `next build` passes with zero errors
- [ ] No `any` types in props or API responses
- [ ] Middleware file is lean and focused
- [ ] Route handlers have proper error responses
- [ ] Streaming works correctly with slow data
