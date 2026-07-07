# Dependencies

## Internal Agents
- **semantic-version-manager**: Version comparison and semver parsing
- **release-manager**: Receives compatibility reports for gate decisions

## External Tools
- **npm/pnpm/yarn**: Package resolution for JS/TS projects
- **pip**: Python dependency resolution
- **cargo**: Rust dependency resolution
- **Dependency-Track**: SBOM analysis

## Runtime Requirements
- Package manager CLI tools installed
- Access to package registries (npm, PyPI, crates.io)
- Project manifest files (package.json, Cargo.toml, requirements.txt)
