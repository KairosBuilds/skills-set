# Workflow

1. **Scan Repository**: Analyze project structure, package files, and existing documentation
2. **Detect Language**: Identify primary programming language and framework
3. **Extract Metadata**: Read package.json, pyproject.toml, Cargo.toml, or equivalent
4. **Generate README**:
   - Title and description from project metadata
   - Badges for CI, coverage, version, license
   - Installation instructions matching project type
   - Usage examples from source code analysis
   - API documentation generation
   - Contribution guidelines
   - License information
5. **Validate**: Check all links, verify code examples compile
6. **Output**: Write README.md to project root
