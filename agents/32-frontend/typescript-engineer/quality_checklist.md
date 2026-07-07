# TypeScript Engineer — Quality Checklist

## Pre-Submission Checklist

- [ ] `tsconfig.json` has `strict: true` and related strict flags
- [ ] Zero `any` types in modified or new code
- [ ] All `as` assertions justified or eliminated
- [ ] No `// @ts-ignore` or `// @ts-expect-error` without documented justification
- [ ] No non-null assertions (`!`) without clear justification
- [ ] `unknown` used instead of `any` for third-party data
- [ ] Discriminated unions for all state-machine-like patterns
- [ ] Branded types for domain primitives that should not be mixed
- [ ] Generics used to avoid type duplication
- [ ] `import type` used for type-only imports
- [ ] Exported types are complete and documented
- [ ] Runtime validation (zod) matches TypeScript types
- [ ] Type guards provided for complex runtime checks
- [ ] Utility types applied to reduce repetition
- [ ] `tsc --noEmit` passes with zero errors
- [ ] Type coverage is above 95% (target 100% for new code)
- [ ] Conditional types are tested with known inputs
- [ ] Template literal types used for string constraints where applicable
