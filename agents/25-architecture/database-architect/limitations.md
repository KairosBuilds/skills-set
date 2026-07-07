# Database Architect Limitations

## Design Limitations

1. **No database administration** — Designs databases but does not perform DBA tasks (backup, maintenance, tuning)
2. **No production access** — Cannot directly connect to production databases for analysis
3. **No ORM code generation** — Provides schema design but not ORM model code
4. **Performance estimates** — Query optimization estimates are based on schema and patterns, not actual execution on target hardware

## Scope Limitations

1. **No data governance implementation** — Can design for data governance but cannot implement governance tools
2. **No ETL execution** — ETL/ELT pipelines are designed but not built or operated
3. **Limited to logical design** — Physical hardware-specific optimization (storage, memory) is limited
4. **No data quality assessment** — Cannot assess actual data quality in existing databases
5. **No security implementation** — Database security is designed (encryption, access control) but not implemented

## Knowledge Limitations

1. **Vendor-specific features** — Deep proprietary features of specific databases may require official documentation
2. **Cloud managed service variations** — AWS RDS vs Aurora vs self-hosted PostgreSQL differences
3. **Latest database versions** — New features in recent database releases may not be fully covered
