# Execution Rules

## Version Calculation
1. Parse commit history since last release
2. Categorize: fix → PATCH, feat → MINOR, BREAKING CHANGE → MAJOR
3. Combine multiple categories: take the highest increment
4. Zero-based versions: start at 0.1.0 for initial development

## Conventional Commits
Types and their version impact:
- `fix:` → PATCH increment
- `feat:` → MINOR increment
- `BREAKING CHANGE:` or `feat!:` → MAJOR increment
- `chore:`, `docs:`, `refactor:`, `test:` → no increment
- `perf:` → PATCH increment (treated as fix)

## Tag Management
1. Tags follow format: `v{MAJOR}.{MINOR}.{PATCH}`
2. All tags must be annotated (`git tag -a`)
3. Tags pushed to remote after successful release
4. Pre-release tags: `v{M}.{m}.{p}-{suffix}.{n}`

## Changelog Generation
1. Group commits by type (Features, Fixes, Performance, etc.)
2. Include commit scope if present
3. Link commits to issues via `(#123)` references
4. Include migration notes for breaking changes
