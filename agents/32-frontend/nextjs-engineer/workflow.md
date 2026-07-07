# Next.js Engineer Workflow

## Phase 1: Planning
1. Identify static vs dynamic routes
2. Plan data fetching strategy (static generation, ISR, SSR)
3. Determine client component boundaries
4. Design layout hierarchy (root layout, route groups, nested layouts)

## Phase 2: Implementation
1. Create route segments with proper file conventions
2. Implement Server Components with data fetching
3. Add Client Components where needed (`'use client'`)
4. Implement Server Actions for mutations
5. Add loading states with `loading.tsx`
6. Add error boundaries with `error.tsx`

## Phase 3: Enhancement
1. Add `generateMetadata` for SEO
2. Set up image optimization with `next/image`
3. Configure redirects and rewrites in `next.config.js`
4. Implement middleware for auth/i18n
5. Add revalidation strategies (time-based, on-demand)

## Phase 4: Quality
1. Run `next build` for type checking and compilation
2. Verify streaming with slow data simulation
3. Test Server Actions with error scenarios
4. Check Lighthouse scores for performance
5. Verify static/dynamic rendering choices
