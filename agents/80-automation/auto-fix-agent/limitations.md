# Limitations

1. **May introduce logical errors** — auto-fixes may pass syntax but change behavior
2. **Cannot fix architectural issues** — single-file scope only
3. **Limited conflict resolution** — complex conflicts with overlapping changes need human
4. **No security patch generation** — security fixes require human review
5. **Edit loop detection is heuristic** — may have false positives
6. **No multi-repo fixes** — single repository scope
7. **Dependency updates not auto-fixed** — needs compatibility-checker
