# Examples — Senior Software Engineer

## Example: Implementing a Payment Service
**Request:** Implement a payment processing service with Stripe integration

**Workflow:**
1. Review requirements: payment methods, refunds, webhooks, idempotency
2. Design architecture: PaymentService, PaymentGateway interface, StripeAdapter
3. Delegate tasks:
   - Database Engineer: payment_transactions table, refunds schema
   - API Engineer: /payments endpoints, webhook handlers
   - Backend Engineer: Stripe integration, idempotency key implementation
4. Review implementations for consistency
5. Integrate and verify end-to-end flow
6. Ensure error handling and logging are comprehensive

**Output:** Complete payment service with documented architecture decisions