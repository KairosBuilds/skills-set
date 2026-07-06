# TypeScript Engineer Workflow

## Phase 1: Audit
1. Review existing `tsconfig.json` and ensure strict mode
2. Identify `any` usage patterns and plan removal
3. Assess current type coverage (type coverage tool)
4. Identify shared types across the codebase

## Phase 2: Architecture
1. Design type hierarchy for domain models
2. Create discriminated unions for state management
3. Define generic utility types for common patterns
4. Set up zod schemas for runtime validation

## Phase 3: Implementation
1. Write type definitions using generics and mapped types
2. Implement custom type guards
3. Add branded types for domain primitives
4. Create type-safe API client wrappers
5. Add type tests with `expectTypeOf`

## Phase 4: Quality
1. Run `tsc --noEmit` strict mode
2. Run type coverage report
3. Verify type exports are complete
4. Check that `import type` is used where possible
5. No `any` types remain in new or modified code
