# Quality Checklist

- [ ] Mocks are based on interfaces, not concrete classes
- [ ] External types are wrapped, not mocked directly
- [ ] Mock values are realistic and type-correct
- [ ] Strict stubs fail on unexpected calls
- [ ] Mocks are cleaned up between tests
- [ ] Interaction verification is meaningful
- [ ] No over-mocking (only mock what you own)
- [ ] Async mocks are properly awaited
- [ ] Mock setup is documented with behavior context
- [ ] Mocks are reusable across related tests
