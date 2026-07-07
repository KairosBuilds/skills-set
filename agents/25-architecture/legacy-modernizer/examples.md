# Legacy Modernizer Examples

## Example 1: Strangler Fig Migration

**Request:** "Modernize our legacy PHP monolith to Node.js microservices"

**Strategy:**
- Phase 1 (Months 1-2): Set up strangler fig interception layer (Nginx + feature flags), route reporting module to new Node.js service
- Phase 2 (Months 3-4): Extract user management module, implement anti-corruption layer for legacy DB access
- Phase 3 (Months 5-6): Extract order processing, implement event-based sync between old and new
- Phase 4 (Months 7-8): Extract remaining modules, redirect all traffic to new system
- Phase 5 (Month 9): Decommission legacy PHP monolith after validation period
- Risk Mitigation: Feature flags allow instant rollback, data validation at every phase, parallel run validation

## Example 2: Database Migration

**Request:** "Migrate from MySQL to PostgreSQL without downtime"

**Strategy:**
- Phase 1: Set up PostgreSQL as replica, continuous sync via Debezium CDC
- Phase 2: Dual-write to both databases (application layer), read from PostgreSQL
- Phase 3: Verify data consistency, run reconciliation jobs
- Phase 4: Remove MySQL dependency, redirect all reads/writes to PostgreSQL
- Phase 5: Decommission MySQL after 30-day validation
- Rollback: Switch application config to MySQL if issues found (keep MySQL in sync)

## Example 3: Technical Debt Reduction

**Request:** "Create a plan to reduce our technical debt"

**Assessment:**
- Current debt: ~180 person-days estimated
- Categories: Test coverage (40%), code quality (30%), architecture issues (20%), outdated dependencies (10%)
- Priority: Architectural debt first (highest risk), then test coverage, then code quality
- Plan: 3 sprints for architectural debt, 6 sprints for test coverage (target 80%), ongoing code quality improvement
- Measurement: SonarQube quality gate, dependency checker, test coverage reports
