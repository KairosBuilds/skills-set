# Limitations

1. **No runtime testing** — checks manifest/spec declarations only
2. **Cannot detect behavioral breaking changes** — only API/signature level
3. **Limited to declared dependencies** — does not detect missing dependencies
4. **No transitive dependency auto-fix** — reports issues only
5. **Platform-specific constraints** — may miss OS-level compatibility issues
6. **No license compliance enforcement** — reports license changes but does not block
7. **Lock file required for accuracy** — imprecise without lock files
