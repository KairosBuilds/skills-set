# Orchestrator Examples

## Example 1: Multi-Agent Architecture Task

**User Request:** "Design a cloud-native microservices platform for our e-commerce application"

**Orchestration Flow:**
1. **Parse** — Intent: architecture design; Domain: e-commerce; Scope: full platform; Format: document + diagrams
2. **Decompose** — Subtasks: (A) System architecture design, (B) Microservices decomposition, (C) Cloud infrastructure design, (D) API design, (E) Database schema design
3. **Route** — (A) system-architect, (B) microservices-architect, (C) cloud-architect, (D) api-designer, (E) database-architect
4. **Execute** — A, B, C in parallel; D depends on B; E depends on A+B
5. **Merge** — Combine outputs into unified architecture document
6. **Validate** — Check consistency: verify microservices boundaries align with database schemas, API contracts match service definitions
7. **Deliver** — Comprehensive architecture document with diagrams, ADRs, and migration plan

## Example 2: Conflict Resolution

**User Request:** "Should we use REST or GraphQL for our new API?"

**Detected Conflict:**
- api-designer recommends REST (maturity, caching, tooling)
- graphql-architect recommends GraphQL (flexibility, reduced over-fetching, single endpoint)

**Resolution:**
- Apply specificity rule: graphql-architect is more specialized for GraphQL decisions
- Apply recency: both analyses are concurrent
- Result: graphql-architect recommendation preferred, but api-designer concerns about caching noted
- Output: Recommendation with documented trade-offs and mitigation strategies for chosen approach

## Example 3: Agent Failure Recovery

**User Request:** "Map our codebase dependencies and identify module boundary violations"

**Orchestration Flow:**
1. **Route** — repository-mapper for codebase analysis
2. **Failure** — repository-mapper returns error: "Unsupported language detected"
3. **Fallback** — Route to dependency-architect with enriched context including the failure reason
4. **Recovery** — dependency-architect fulfills the task with manual dependency analysis
5. **Log** — Record repository-mapper limitation for future routing decisions

## Example 4: Simple Single-Agent Task

**User Request:** "Create an ADR for our PostgreSQL database selection"

**Orchestration Flow:**
1. **Parse** — Intent: ADR creation; Domain: database; Scope: single decision
2. **Route** — Directly to solution-architect
3. **Validate** — Verify ADR format includes all required sections
4. **Deliver** — Complete ADR document
