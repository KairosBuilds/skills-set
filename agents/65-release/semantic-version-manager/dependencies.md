# Dependencies

## Internal Agents
- **release-manager**: Receives version information for release pipeline
- **compatibility-checker**: Validates dependency versions align

## External Tools
- **Git**: Tag creation and commit history reading
- **semantic-release**: Automated versioning (optional integration)
- **conventional-changelog**: Changelog format library

## Runtime Requirements
- Git CLI with push access to remote
- Commit history following conventional commits
- Project version files accessible (package.json, Cargo.toml, etc.)
