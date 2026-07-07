# Dependencies

## Internal Agents
- **release-manager**: Coordinates migration timing with releases
- **compatibility-checker**: Validates schema compatibility with app

## External Tools
- **Database CLI**: psql, mysql, sqlcmd
- **Migration Framework**: Flyway, Liquibase, Alembic, Prisma Migrate
- **Backup Tooling**: pg_dump, mysqldump

## Runtime Requirements
- Database access credentials (read/write)
- Migration tooling installed
- Rollback scripts generated before execution
