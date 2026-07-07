# Examples

## PostgreSQL Query Analysis
```sql
-- Before optimization
EXPLAIN ANALYZE SELECT * FROM orders WHERE user_id = 123 ORDER BY created_at DESC;
-- Seq Scan on orders (cost=0.00..4500.00 rows=500 width=120)
-- Actual Time: 245ms

-- After adding index
CREATE INDEX CONCURRENTLY idx_orders_user_created ON orders(user_id, created_at DESC);
-- Actual Time: 2ms
```

## MongoDB Index
```javascript
db.orders.createIndex({ userId: 1, createdAt: -1 });
db.orders.find({ userId: 123 }).sort({ createdAt: -1 }).explain('executionStats');
```
