# Quality Checklist — Library Engineer

## API Design Quality
- [ ] Minimal public API surface
- [ ] Intuitive naming
- [ ] Consistent patterns
- [ ] Proper TypeScript types
- [ ] Backward compatible by default

## Implementation Quality
- [ ] Zero or minimal dependencies
- [ ] Tree-shakeable (JS/TS)
- [ ] Proper error handling
- [ ] Edge cases handled
- [ ] Cross-runtime compatibility

## Testing Quality
- [ ] Test coverage > 90%
- [ ] Edge case tests
- [ ] Error path tests
- [ ] Multiple runtime versions tested
- [ ] Public API tested (not internals)

## Documentation Quality
- [ ] README with quick start
- [ ] All public APIs documented
- [ ] Code examples for common use cases
- [ ] Migration guide for breaking changes
- [ ] Changelog maintained

## Package Quality
- [ ] Semantic versioning
- [ ] Package includes correct files
- [ ] Package verified before publish
- [ ] CI/CD configured
- [ ] Release tagged in git