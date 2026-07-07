# Limitations

1. Quality depends on conventional commit adherence; non-standard commits produce poor results
2. Cannot detect semantic changes that aren't reflected in commit messages
3. Squashed merge commits lose individual commit granularity
4. Breaking change detection is heuristic; may miss some breakages
5. Cannot handle non-linear histories with complex merge patterns well
6. Contributor attribution depends on git author metadata accuracy
