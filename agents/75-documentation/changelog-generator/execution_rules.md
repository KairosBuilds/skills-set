# Execution Rules

1. Parse git log using conventional commit format (feat:, fix:, chore:, etc.)
2. Group changes by type (Features, Bug Fixes, Documentation, etc.)
3. Identify breaking changes from commits with ! or BREAKING CHANGE footer
4. Calculate semver bump based on commit types
5. Preserve existing CHANGELOG entries; prepend new release
6. Include contributor attribution when available
7. Handle merge commits and squashed commits correctly
8. Validate that version tags match semver format
