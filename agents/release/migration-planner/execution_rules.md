# Execution Rules

## Safety First
1. Always generate rollback scripts before running migrations
2. Back up data before destructive operations (DROP, ALTER, DELETE)
3. Test migrations on staging before production
4. Estimate downtime window and communicate to stakeholders

## Migration Types
1. **Schema Migrations**: Additive changes preferred; avoid destructive ALTERs
2. **Data Migrations**: Batched with progress tracking and resume capability
3. **Platform Migrations**: Strangler Fig pattern for legacy systems

## Validation Rules
1. Verify data integrity before and after migration
2. Run compatibility checks against dependent services
3. Validate foreign key constraints after schema changes
4. Check index performance after migration

## Rollback Protocol
1. Rollback must restore original schema and data
2. Test rollback on staging before production
3. Rollback window: 2× migration time or 30min max
