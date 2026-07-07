# Microservices Architect Examples

## Example 1: E-Commerce Monolith Decomposition

**Request:** "Decompose our e-commerce monolith into microservices"

**Output:**
- Domain Analysis: Identified 7 bounded contexts — Product Catalog, Shopping Cart, Order Management, Payment, Inventory, User Account, Notification
- Service Identification: 7 microservices matching bounded contexts
- Communication: Async events for order status changes, inventory updates; sync REST for queries
- Data Ownership: Each service gets its own PostgreSQL schema initially, migrating to separate databases
- Saga: Order creation saga — Reserve Inventory → Process Payment → Confirm Order → Notify Customer
- Migration Plan: Strangler fig pattern over 6 months, starting with Notification and Inventory services

## Example 2: Service Boundary Validation

**Request:** "Review our service boundaries for anti-patterns"

**Analysis:**
- Issue: Order and Payment services share a database — violates service autonomy
- Issue: User service handles both authentication and notification — violates single responsibility
- Issue: Circular dependency between Cart and Order services
- Recommendations: Split notification into dedicated service, decouple Cart and Order with async events

## Example 3: Communication Pattern Design

**Request:** "Design inter-service communication for our booking platform"

**Output:**
- Sync: Booking queries, availability checks via gRPC (low latency required)
- Async: Booking confirmation, payment processing, notification via Kafka
- Events schema defined for: BookingCreated, PaymentProcessed, BookingConfirmed, BookingCancelled
- Saga: Booking flow with compensating transactions for failures
- Error handling: Dead letter queues, retry policies with exponential backoff
