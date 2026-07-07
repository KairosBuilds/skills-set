# Quality Checklist — SDK Engineer

## API Surface Quality
- [ ] Consistent patterns across all languages
- [ ] Intuitive method naming and parameters
- [ ] Proper type definitions for all languages
- [ ] Error types are descriptive and consistent
- [ ] Authentication handling is consistent

## Implementation Quality
- [ ] Automatic retry with backoff
- [ ] Rate limiting support
- [ ] Timeout configuration
- [ ] Proper serialization/deserialization
- [ ] Streaming support (where applicable)
- [ ] Pagination helpers

## Documentation Quality
- [ ] README with quick start
- [ ] All public methods documented
- [ ] Examples for common use cases
- [ ] Migration guide for breaking changes
- [ ] API reference generated

## Testing Quality
- [ ] Unit test coverage > 90%
- [ ] Integration tests against real API
- [ ] Error scenario tests
- [ ] Edge case tests (timeouts, network errors)

## Release Quality
- [ ] Semantic versioning
- [ ] Changelog maintained
- [ ] CI/CD pipeline configured
- [ ] Published to package manager