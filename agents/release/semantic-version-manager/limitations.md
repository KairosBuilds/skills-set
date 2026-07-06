# Limitations

1. **Requires conventional commits** — non-standard messages may cause incorrect bumps
2. **No multi-package references** — monorepo support requires per-package tags
3. **Cannot detect actual breaking changes** — relies on commit message convention
4. **No pre-release channels** — only stable version management
5. **Manual override needed** — for semantic conflicts (e.g., breaking change labeled as feat)
6. **Unicode in commit messages** — limited support for non-ASCII
7. **No backport versioning** — hotfix branches need manual version assignment
