# Database Architect Examples

## Example 1: E-Commerce Schema Design

**Request:** "Design a database schema for an e-commerce platform"

**Output:**
- Tables: users, products, categories, orders, order_items, reviews, payments, shipments
- Relationships: User 1:N Order, Order 1:N OrderItems, Product 1:N OrderItems, Product N:M Category
- Indexes: Composite index on (user_id, created_at) for order history, (product_id, rating) for top-rated products
- Partitioning: orders table partitioned by month, reviews table partitioned by product_id hash
- Constraints: CHECK price > 0, UNIQUE (user_id, product_id) for reviews
- DDL statements for all tables with auto-generated documentation

## Example 2: Query Optimization

**Request:** "Our dashboard query is slow (45 seconds). Optimize it."

**Original Query:**
```sql
SELECT u.name, COUNT(o.id) as order_count, SUM(o.total) as total_spent
FROM users u
LEFT JOIN orders o ON u.id = o.user_id
WHERE o.created_at >= '2025-01-01'
GROUP BY u.id
ORDER BY total_spent DESC
LIMIT 100;
```

**Optimization:**
- Issue: Full table scan on users, no index on o.created_at for join order
- Added composite index: (o.user_id, o.created_at, o.total)
- Rewritten to INNER JOIN (since WHERE filters orders)
- Result: 45s → 0.3s

## Example 3: Database Selection

**Request:** "Should we use PostgreSQL or MongoDB for our content management system?"

**Analysis:**
- Requirements: Complex relationships (content tree, taxonomies), search, flexible metadata, moderate scale
- PostgreSQL: Superior for relationships via foreign keys, JSONB for flexible metadata, full-text search, mature tooling
- MongoDB: Flexible schema, easier horizontal scaling, built-in aggregation pipeline
- Recommendation: PostgreSQL with JSONB for metadata — best balance of relational integrity and schema flexibility
- ADR documenting decision with trade-offs
