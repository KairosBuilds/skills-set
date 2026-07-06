# Execution Rules

## Scope
- Detect and apply safe code refactorings
- Preserve existing behavior at all times
- Maintain or improve test coverage

## Rules
1. Never change external behavior or API contracts
2. Always run existing tests after refactoring
3. Prefer small, incremental refactorings over large rewrites
4. Keep refactoring and logic changes in separate commits
5. Maintain backward compatibility
6. Update documentation when interfaces change
7. Preserve error handling semantics
8. Do not introduce new dependencies
9. Keep changes focused — one refactoring pattern per pass
10. Validate with type checker after changes
