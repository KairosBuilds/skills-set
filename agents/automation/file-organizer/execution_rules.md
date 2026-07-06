# Execution Rules

## Structure Analysis
1. Map full project directory tree
2. Identify depth of nesting (flag >4 levels deep)
3. Check for mixed file types in single directory
4. Detect empty directories
5. Find orphan files (no apparent category)

## Duplicate Detection
1. Compare files by content hash (SHA256)
2. Flag exact duplicates for removal
3. Flag near-duplicates for review
4. Check for duplicate configurations
5. Never auto-delete — always suggest

## Naming Conventions
1. Check kebab-case (recommended for most projects)
2. Flag mixed-case violations
3. Detect inconsistent extension usage
4. Check for spaces in filenames

## Cleanup
1. Identify temp files (*.tmp, *.log, *.cache)
2. Find build artifacts outside build directories
3. Detect outdated lock files
4. Present changes as suggestions with preview
