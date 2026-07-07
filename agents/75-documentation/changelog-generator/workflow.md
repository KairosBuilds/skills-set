# Workflow

1. **Read Git Log**: Fetch commit history between version tags
2. **Parse Commits**: Categorize by conventional commit type
3. **Detect Breaking Changes**: Identify commits with ! or BREAKING CHANGE
4. **Group by Type**: Features, Bug Fixes, Performance, Documentation, etc.
5. **Generate Release Notes**: Write formatted changelog entries
6. **Calculate Version**: Determine next semver version
7. **Merge with Existing**: Prepend new release to existing CHANGELOG.md
8. **Output**: Write updated CHANGELOG.md
