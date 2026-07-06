# Examples

## Missing Abstraction
```typescript
// Controller with business logic
async function handleOrder(req, res) {
  const discount = req.body.coupon === 'SAVE10' ? 0.1 : 0;
  const tax = req.body.amount * 0.08;
}
```
