# Limitations

1. **Cannot restructure symlinked directories** — follows links, does not reorganize
2. **No intelligent grouping by content** — filename and extension based only
3. **Cannot detect semantic duplicates** — different names, same content
4. **No git-aware operations** — does not consider git history
5. **Suggestions only** — no automatic restructuring without approval
6. **Large repos may be slow** — full directory scan needed
7. **No cross-project organization** — single project scope
