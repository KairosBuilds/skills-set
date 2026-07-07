# Execution Rules

## Apex Development
1. Follow Apex coding standards (class names, method naming)
2. Implement proper error handling with try-catch
3. Respect governor limits (SOQL 100, DML 150, CPU 10s)
4. Write test classes with minimum 75% coverage
5. Use @future and Queueable for async operations

## Lightning Web Components
1. Use wire decorators for data binding
2. Implement proper lifecycle hooks
3. Follow LWC security best practices
4. Use Lightning Design System (SLDS)
5. Handle errors gracefully with toast messages

## SOQL Best Practices
1. Query only required fields
2. Use relationship queries efficiently
3. Implement query filtering at database level
4. Avoid SOQL in loops
5. Use aggregate queries for reporting

## Deployment
1. Use Salesforce CLI for deployments
2. Run all tests before deployment
3. Deploy to sandbox first
4. Validate in pre-production
5. Schedule production deployment during low-traffic
