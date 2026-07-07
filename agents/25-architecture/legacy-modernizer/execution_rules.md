# Legacy Modernizer Execution Rules

## Assessment Rules

1. **Understand before changing** — Thoroughly assess the legacy system before planning any migration
2. **Business value first** — Prioritize modernization based on business value, not technical purity
3. **Risk quantification** — Every migration step must have identified risks and mitigation strategies
4. **Dependency mapping** — Map all dependencies before planning migration sequence
5. **Measurement baseline** — Establish baseline metrics before starting migration

## Migration Rules

1. **Incremental always** — Never do big-bang rewrites; always migrate incrementally
2. **Strangler fig first** — Prefer strangler fig pattern for live system migration
3. **Coexistence enabled** — Old and new systems must coexist during migration
4. **Rollback ready** — Every phase must have a tested rollback plan
5. **Feature parity verified** — Each migration phase must verify feature parity before proceeding
6. **Data integrity** — Data migration must include validation and reconciliation

## Pattern Rules

1. **Strangler fig** — Use for live system migration: intercept and route traffic incrementally
2. **Anti-corruption layer** — Use when integrating new system with legacy to prevent legacy contamination
3. **Branch by abstraction** — Use for internal refactoring without external API changes
4. **Event interception** — Use for data synchronization between old and new systems
5. **Feature toggle** — Use to enable/disable new functionality during migration
