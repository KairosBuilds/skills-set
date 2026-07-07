# Execution Rules — PHP Engineer

## General Rules
1. MUST use declare(strict_types=1) on all files
2. MUST use type hints for all function parameters and returns
3. MUST use PHP 8.3+ features (enums, readonly classes, etc.)
4. MUST write tests with PHPUnit or Pest
5. MUST use Composer for dependency management

## Symfony Rules
1. Use autowiring for dependency injection
2. Implement proper service configuration
3. Use Symfony Messenger for async tasks
4. Implement proper event subscribers
5. Use Doctrine ORM for database access

## Security Rules
1. Use password hashing (password_hash/bcrypt)
2. Sanitize all user input
3. Use prepared statements or ORM for queries
4. Implement CSRF protection
5. Validate file uploads