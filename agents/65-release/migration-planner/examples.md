# Examples

## Example 1: Schema Migration
```
Input: "Add email_verified column to users table"
Actions:
1. Generate ALTER TABLE script
2. Create rollback (DROP COLUMN)
3. Set default value for existing rows
4. Add index on new column
5. Test on staging with 100k rows
6. Schedule 5min maintenance window
7. Execute and verify
```

## Example 2: Data Migration
```
Input: "Migrate user preferences from JSON to normalized tables"
Actions:
1. Create user_preferences table
2. Write ETL script (batched 1000 rows)
3. Generate rollback (INSERT back to JSON column)
4. Test data integrity: random sample comparison
5. Execute in batches with progress logging
6. Verify row counts match
```

## Example 3: Platform Migration
```
Input: "Migrate from MySQL to PostgreSQL"
Actions:
1. Schema mapping analysis
2. Data type compatibility check
3. Strangler Fig: dual-write phase
4. Data export/import with verification
5. Cutover with DNS switch
6. Rollback plan: DNS revert
```
