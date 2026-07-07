# React Engineer — Quality Checklist

## Pre-Submission Checklist

- [ ] TypeScript strict mode — no `any`, no implicit `any`
- [ ] Proper error boundaries implemented for data-fetching sections
- [ ] Suspense boundaries used for async operations
- [ ] Loading, empty, and error states all handled
- [ ] Event handlers wrapped with `useCallback` where appropriate
- [ ] Expensive computations memoized with `useMemo`
- [ ] No unnecessary re-renders (verify with React DevTools)
- [ ] Server/Client component split is optimal
- [ ] Keyboard navigation works for interactive elements
- [ ] Screen reader labels present on all interactive elements
- [ ] ARIA attributes correct and complete
- [ ] Component tree depth reasonable (no prop drilling without context)
- [ ] All hooks follow Rules of Hooks (no conditional hooks)
- [ ] Cleanup functions provided in `useEffect`
- [ ] Dependencies array in `useEffect` is correct
- [ ] `npm run typecheck` passes
- [ ] `npm run lint` passes
- [ ] Unit tests pass with >80% coverage
- [ ] Responsive design verified at mobile, tablet, desktop breakpoints
