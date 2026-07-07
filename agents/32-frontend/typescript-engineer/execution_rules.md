# Execution Rules for TypeScript Engineer Agent

## Core Rules

1. **Strict Mode**: Always enable `strict: true` in `tsconfig.json`. Include `noUncheckedIndexedAccess`, `exactOptionalPropertyTypes`, `noPropertyAccessFromIndexSignature` where appropriate.
2. **No `any`**: Never use `any`. Use `unknown` and type narrowing. If third-party library lacks types, create `.d.ts` declarations.
3. **Generics**: Use generics over type assertions. Prefer generic constraints with `extends`.
4. **Branded Types**: Use branded/nominal types for domain primitives (e.g., `UserId`, `Email`) to prevent type confusion.
5. **Discriminated Unions**: Model state machines and API responses with discriminated unions.
6. **Type Guards**: Write user-defined type guards (`x is T`) for runtime validation. Use zod for runtime schema validation.
7. **Template Literal Types**: Use template literal types for string patterns and CSS-like values.
8. **Mapped Types**: Prefer mapped and conditional types over repetitive manual type definitions.
9. **Utility Types**: Leverage built-in `Partial`, `Pick`, `Omit`, `Exclude`, `Extract`, `ReturnType`, `Awaited`.
10. **Exports**: Export types and interfaces explicitly. Use `import type` for type-only imports.

## Prohibited

- `any` type (use `unknown` instead)
- `as` assertions without prior `instanceof` or type guard check
- `// @ts-ignore` or `// @ts-expect-error` without documented reason
- `Function` type (use proper function signatures)
- `object` type (use `Record<string, unknown>` or proper interface)
- `* as x` namespace imports for types
- Non-null assertion `!` without justification

## Enforcement

`tsc --noEmit` must pass with strict mode before task completion.
