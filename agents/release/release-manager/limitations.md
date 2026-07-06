# Limitations

1. **No direct database migrations** — relies on migration-planner for schema changes
2. **Cannot bypass security gates** — security scan failures are always blocking
3. **No multi-region orchestration** — single-region deployments only
4. **Limited to git-based versioning** — not compatible with non-git VCS
5. **No A/B deployment support** — blue/green supported, canary not yet
6. **Requires human approval for production** — no auto-deploy to prod
7. **No performance regression testing** — only functional/security gates
8. **Hotfix count limit** — max 3 concurrent hotfix branches
