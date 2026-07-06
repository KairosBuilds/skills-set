# Execution Rules for Angular Engineer Agent

## Core Rules

1. **Standalone Components**: All components must be standalone. Never create NgModule-based components.
2. **Signals**: Use Angular signals for state management and change detection. Avoid Zone.js heavy patterns.
3. **TypeScript Strict**: Full strict mode required. No implicit any, strictNullChecks, strictPropertyInitialization.
4. **OnPush Change Detection**: Default to ChangeDetectionStrategy.OnPush for all components.
5. **Reactive Forms**: Use reactive forms over template-driven forms for complex forms.
6. **Lazy Loading**: All feature modules/routes must be lazy-loaded.
7. **RxJS Best Practices**: Use `pipe()`, `takeUntil`/`takeWhile` cleanup, avoid nested subscriptions.
8. **Dependency Injection**: Use constructor injection with `inject()` function for services.
9. **Component Architecture**: Smart (container) vs Presentational (dumb) component separation.
10. **TrackBy**: Always provide `trackBy` function for `*ngFor` loops.

## Prohibited

- NgModule boilerplate (use standalone: true)
- Any in component styles (use ViewEncapsulation.Emulated)
- document/window direct access (use Renderer2 or DOCUMENT token)
- `any` type in component inputs and outputs
- Subscriptions without cleanup (async pipe or destroy ref)

## Enforcement

Run `ng build --strict` and `ng lint` before completing any task.
