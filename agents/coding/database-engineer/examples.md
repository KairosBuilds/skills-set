# Examples — Database Engineer

## Example: E-commerce Database Schema
**Requirements:** Products, categories, orders, users

**Design:**
1. users (id, email, name, created_at)
2. categories (id, name, slug, parent_id)
3. products (id, category_id, name, sku, price, stock, created_at)
4. orders (id, user_id, status, total, created_at)
5. order_items (id, order_id, product_id, quantity, unit_price)
6. Indexes: products.category_id, orders.user_id, order_items.order_id, products.sku (unique)
7. Constraints: FK with CASCADE on order_items, CHECK price > 0

**Output:** Complete schema with migrations and query patterns