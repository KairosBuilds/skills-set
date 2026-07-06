# Execution Rules — Django Engineer

## General Rules
1. MUST follow Django's app-based architecture
2. MUST use Django ORM for database access
3. MUST use Django's built-in admin for data management
4. MUST write tests with pytest-django
5. MUST use Django's form/DRF serializer for validation

## Model Rules
1. Use verbose_name and verbose_name_plural for model metadata
2. Implement __str__ for all models
3. Use class Meta for ordering and constraints
4. Use db_index for frequently queried fields
5. Use related_name for reverse relationships

## DRF Rules
1. Use ViewSets and ModelViewSets for CRUD
2. Implement proper serializer validation
3. Use permissions classes for authorization
4. Use pagination for list endpoints
5. Use filtering backends for search/filter

## Performance Rules
1. Use select_related/prefetch_related for related data
2. Use only/defer for specific field selection
3. Use database-level aggregations
4. Implement caching with Django cache framework
5. Use Celery for long-running tasks