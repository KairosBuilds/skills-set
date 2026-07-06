# Angular Engineer — Quality Checklist

## Pre-Submission Checklist

- [ ] All components are standalone with `standalone: true`
- [ ] OnPush change detection applied to all components
- [ ] Signals used for local state where appropriate
- [ ] No `any` types in component inputs/outputs
- [ ] All subscriptions cleaned up (async pipe, takeUntil, or DestroyRef)
- [ ] `trackBy` function provided for all `*ngFor` loops
- [ ] Lazy loading configured for all feature routes
- [ ] Route guards implemented for protected routes
- [ ] Reactive forms with proper validation
- [ ] Error handling for all HTTP requests
- [ ] Loading, empty, error states for all async views
- [ ] `inject()` function used over constructor injection
- [ ] NgRx feature states lazy-loaded (if using NgRx)
- [ ] `ng build --strict` passes with zero errors
- [ ] ESLint with Angular rules passes
- [ ] Unit tests pass for services, components, and pipes
- [ ] Responsive design verified
- [ ] Bundle size reviewed (no unnecessary imports)
