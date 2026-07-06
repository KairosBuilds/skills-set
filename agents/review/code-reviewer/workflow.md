# Workflow

1. **Ingestion** — Receive PR diff or file list for review
2. **Parsing** — Parse language-specific AST or use regex-based pattern matching
3. **Analysis** — Run configured checks: security, performance, style, naming, architecture
4. **Classification** — Severity-tag each finding using rubric
5. **Reporting** — Generate structured markdown report grouped by severity
6. **Feedback** — Present results with inline suggestions and code examples
