# Examples

## Example 1: Structure Suggestion
```
Input: "Organize my project files"
Report:
- src/ has 3 subdirectories, 45 loose files
- Suggestion: group by feature module
  - src/components/ (12 files)
  - src/utils/ (8 files)
  - src/hooks/ (5 files)
  - src/types/ (4 files)
- 3 empty directories found → remove
```

## Example 2: Duplicate Detection
```
Input: "Find duplicate files"
Duplicates Found:
1. config.dev.json == config.development.json (identical)
2. styles.css (src/) == styles.css (lib/) (identical)
3. logo.png v1, logo.png v2 (similar, 95% match)
```

## Example 3: Cleanup
```
Input: "Clean up temporary files"
Files to Remove:
- 12 .log files in project root (12MB)
- 8 .tmp files in src/ (4MB)
- old package-lock.json (backup from 3 versions ago)
Total: 22 files, 18MB reclaimed
```
