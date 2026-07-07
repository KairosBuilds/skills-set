# Execution Rules

## Setup Discovery
1. Check for ONBOARDING.md, README.md, CONTRIBUTING.md
2. Detect project type (package.json, Cargo.toml, pyproject.toml, setup.py)
3. Identify package manager (npm, pnpm, yarn, pip, cargo)
4. Check for Docker/devcontainer configuration

## Dependency Installation
1. Use correct package manager for project
2. Install production and dev dependencies
3. Verify lock file exists and is up-to-date
4. Handle version conflicts gracefully

## Environment Verification
1. Check Node.js/Python/Rust version compatibility
2. Verify build succeeds
3. Check tests pass (basic smoke test)
4. Verify LSP/linter configuration
5. Confirm all required tools are installed

## Troubleshooting
1. Analyze error messages from failed steps
2. Check common issues (node version, missing build tools)
3. Suggest fixes for detected problems
4. Rollback failed setup attempts
5. Escalate unresolvable issues
