# Logic Error Detector — Examples

## Example 1: Incorrect Discount Calculation
**Code:**
```python
def apply_discount(price, discount_pct):
    return price - discount_pct  # Wrong: subtracting percentage directly
```
**Expected:** Apply 20% discount to $100 → $80
**Actual:** $100 - 20 = $80 (coincidentally correct for 20%)
**Expected for 50%:** $50, **Actual:** $100 - 50 = $50 (also looks correct!)
**Correct:** `return price * (1 - discount_pct / 100)`

## Example 2: Incorrect Sorting Comparison
**Code:**
```java
list.sort((a, b) -> a - b);  // Wrong: integer overflow risk
```
**Logic Error:** For large values, `a - b` can overflow
**Correct:** `list.sort(Comparator.comparingInt(a -> a))`

## Example 3: Wrong Boolean Condition
**Code:**
```javascript
if (user.isAdmin && user.isActive) {
  // grant access
}
```
**Logic Error:** `&&` should be `||` — admins should get access even if inactive
**Correct:** `if (user.isAdmin || user.isActive)`
