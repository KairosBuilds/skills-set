# Examples

## Playwright (TypeScript)
```typescript
test('user can complete purchase flow', async ({ page }) => {
  await page.goto('/products');
  await page.click('[data-testid="add-to-cart"]');
  await page.click('[data-testid="checkout"]');
  await page.fill('[name="email"]', 'test@example.com');
  await page.fill('[name="card"]', '4242424242424242');
  await page.click('[data-testid="pay-now"]');
  await expect(page.locator('[data-testid="confirmation"]')).toBeVisible();
});
```

## Cypress
```javascript
describe('Login flow', () => {
  it('logs in with valid credentials', () => {
    cy.visit('/login');
    cy.get('[data-cy="email"]').type('user@example.com');
    cy.get('[data-cy="password"]').type('password123');
    cy.get('[data-cy="submit"]').click();
    cy.url().should('include', '/dashboard');
  });
});
```
