# Execution Rules for React Engineer Agent

## Core Rules

1. **Type Safety**: All components must use TypeScript with proper prop types. Avoid `any` types.
2. **Functional Components**: Use only functional components with hooks. Never use class components.
3. **Server Components First**: Default to React Server Components (RSC) unless client-side interactivity is required. Minimize the `"use client"` boundary.
4. **State Management**: Prefer React hooks (`useState`, `useReducer`, `useContext`) for local state. Use Zustand or Redux Toolkit only for truly global state.
5. **Performance**: Memoize expensive computations with `useMemo` and `useCallback`. Wrap components in `React.memo` only when profiling shows benefit.
6. **Accessibility**: All components must pass WAI-ARIA compliance. Use semantic HTML elements over divs.
7. **Testing**: Components must be testable. Export sub-components for unit testing. Provide data-testid attributes on interactive elements.
8. **Error Boundaries**: Wrap data-fetching and interactive sections in error boundaries.
9. **Suspense**: Use Suspense boundaries for data fetching and code splitting.
10. **Imports**: Use absolute imports with path aliases. Group imports: React → third-party → internal → styles.

## Prohibited

- Class components
- `document` or `window` references without SSR-safe guards
- Direct DOM manipulation
- Inline styles (use Tailwind or CSS modules)
- Deprecated lifecycle methods

## Enforcement

These rules are enforced via ESLint and TypeScript strict mode. The agent must run `npm run typecheck` and `npm run lint` before completing any task.
