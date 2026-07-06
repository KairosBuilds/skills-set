# Supported Languages

All languages supported.

| Language | Build | Lint | Typecheck |
|----------|-------|------|-----------|
| TypeScript | tsc/esbuild | ESLint | tsc --noEmit |
| JavaScript | esbuild/webpack | ESLint | - |
| Python | setuptools/poetry | Ruff | mypy/pyright |
| Rust | cargo build | Clippy | rustc |
| Go | go build | golangci-lint | go vet |
| Java | mvn/gradle | Checkstyle | javac |
