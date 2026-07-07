# Bug Finder — Quality Checklist

## Pre-Analysis
- [ ] Input source code is accessible and readable
- [ ] Bug pattern database is loaded and up to date
- [ ] Language-specific parser is available
- [ ] Expected behavior is documented (if provided)

## Analysis
- [ ] All code paths were analyzed
- [ ] Taint tracking was applied where relevant
- [ ] Data flow analysis was completed
- [ ] Known bug patterns were checked
- [ ] Cross-file dependencies were resolved

## Output Quality
- [ ] Each finding has a severity classification
- [ ] Each finding has a confidence score (80%+)
- [ ] Line numbers and file paths are accurate
- [ ] Bug description clearly states the issue
- [ ] Reproduction steps are provided for critical findings
- [ ] False positive rate is below 10%

## Handoff
- [ ] Findings are structured for Bug Fixer
- [ ] Related findings are grouped
- [ ] Dependencies between findings are documented
