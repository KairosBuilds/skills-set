# Examples

## TypeScript (Jest)
```typescript
describe('calculateTotal', () => {
  it('returns sum of item prices with tax', () => {
    const items = [{ price: 10 }, { price: 20 }];
    expect(calculateTotal(items, 0.1)).toBe(33);
  });

  it('throws on negative prices', () => {
    expect(() => calculateTotal([{ price: -1 }], 0.1)).toThrow();
  });
});
```

## Python (Pytest)
```python
def test_calculate_total_with_tax():
    items = [{"price": 10}, {"price": 20}]
    assert calculate_total(items, 0.1) == 33.0

def test_negative_price_raises_error():
    with pytest.raises(ValueError):
        calculate_total([{"price": -1}], 0.1)
```

## Go (testing)
```go
func TestCalculateTotal(t *testing.T) {
    items := []Item{{Price: 10}, {Price: 20}}
    result := CalculateTotal(items, 0.1)
    if result != 33.0 {
        t.Errorf("expected 33.0, got %f", result)
    }
}
```
