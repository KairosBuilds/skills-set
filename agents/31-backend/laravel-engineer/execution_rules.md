# Execution Rules — Laravel Engineer

## General Rules
1. MUST use Eloquent ORM for database access
2. MUST use Laravel's validation system
3. MUST use Laravel's policy system for authorization
4. MUST write tests with Pest or PHPUnit
5. MUST use Artisan CLI for code generation

## Eloquent Rules
1. Use  and  for serialization control
2. Use eager loading (with()) to prevent N+1
3. Use scope methods for query encapsulation
4. Use accessors and mutators for attribute transformation
5. Use relationship methods properly (hasMany, belongsTo, etc.)

## API Rules
1. Use API resources for response transformation
2. Use form requests for validation
3. Use API resource collections for lists
4. Implement proper exception handling in API responses
5. Use API versioning for public APIs