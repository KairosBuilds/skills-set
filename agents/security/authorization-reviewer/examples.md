# Examples

## IDOR Vulnerability
```python
def get_order(order_id):
    return Order.objects.get(id=order_id)  # No user check
```
