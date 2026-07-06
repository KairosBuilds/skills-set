# Execution Rules — Python Engineer

## General Rules
1. MUST use type hints for all function signatures and data models
2. MUST use async/await for I/O-bound operations
3. MUST write tests with pytest (not unittest)
4. MUST use Pydantic for data validation
5. MUST follow PEP 8 and use black/ruff formatting

## FastAPI Rules
1. Use dependency injection for shared logic
2. Implement proper response models with Pydantic
3. Use path operations with proper HTTP methods
4. Implement proper exception handlers

## Django Rules
1. Use class-based views for complex views
2. Implement serializer validation
3. Use select_related/prefetch_related for performance
4. Follow Django's model-view-template pattern