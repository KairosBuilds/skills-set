# Examples

## CI Regression Trigger (GitHub Actions)
```yaml
jobs:
  regression:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: npm ci
      - run: npm run test:regression
      - uses: actions/upload-artifact@v4
        if: failure()
        with:
          name: regression-report
          path: reports/regression/
```

## Selective Regression
```bash
# Run only tests in affected modules
npx jest --listTests --findRelatedTests src/changed-file.ts
npx jest --selectProjects unit integration --bail 3
```
