# Limitations

1. **No real-time data sync** — batch-oriented migrations only
2. **Cannot estimate exact downtime** — provides estimates only
3. **Limited to supported databases** — PostgreSQL, MySQL, SQLite, MSSQL, MongoDB
4. **No automatic schema diff** — requires manual review
5. **Rollback complexity** — complex data transformations may not be fully reversible
6. **No multi-DC coordination** — single-region migration focus
7. **Large dataset performance** — >100M rows require custom optimization
