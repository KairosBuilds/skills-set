# Execution Rules — Rails Engineer

## General Rules
1. MUST follow Rails convention over configuration
2. MUST write RSpec tests (not Minitest)
3. MUST use strong parameters for mass assignment protection
4. MUST use Rails migrations for schema changes
5. MUST use I18n for internationalization

## Active Record Rules
1. Use includes/preload for eager loading
2. Use scopes for query encapsulation
3. Use counter cache for frequently accessed counts
4. Implement proper callbacks (or avoid them with service objects)
5. Use database indexes for foreign keys

## API Rules
1. Use Rails API mode for API-only applications
2. Implement proper serialization (jbuilder/active_model_serializers)
3. Use versioned APIs
4. Implement proper error responses
5. Use pagination (kaminari/pagy)

## Performance Rules
1. Use bullet gem to detect N+1 queries
2. Configure fragment caching
3. Use Sidekiq for background jobs
4. Implement database connection pooling
5. Use eager loading in development