# React Engineer Workflow

## Phase 1: Analysis
1. Parse requirements and identify component tree
2. Determine server vs client component boundaries
3. Plan state management approach (local vs global)
4. Identify data fetching patterns (server fetch, React Query, SWR)

## Phase 2: Scaffolding
1. Create component directory structure
2. Define TypeScript interfaces and types
3. Set up Storybook stories (if applicable)
4. Create CSS module or Tailwind utilities

## Phase 3: Implementation
1. Build base component with proper typing
2. Implement state and effects
3. Add event handlers and callbacks
4. Write data fetching logic
5. Add loading, error, empty states

## Phase 4: Optimization
1. Profile with React DevTools
2. Apply memoization where needed
3. Implement code splitting with `lazy()` and `Suspense`
4. Optimize re-renders

## Phase 5: Review
1. Run TypeScript type checking
2. Run ESLint
3. Verify accessibility (axe-core)
4. Write unit tests (Jest/Vitest + Testing Library)
5. Verify responsive behavior
