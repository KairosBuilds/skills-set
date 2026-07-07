# Examples

## Axe Integration (Playwright)
```typescript
import { injectAxe, checkA11y } from 'axe-playwright';

test('homepage has no a11y violations', async ({ page }) => {
  await page.goto('/');
  await injectAxe(page);
  const results = await checkA11y(page, null, {
    includedImpacts: ['critical', 'serious'],
  });
  expect(results.violations).toEqual([]);
});
```

## Lighthouse CI
```bash
lighthouse-ci https://example.com \
  --score=100 --budget=performance \
  --collect.psiStrategy=desktop
```
