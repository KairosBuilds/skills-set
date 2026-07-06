# Legacy Modernizer Workflow

## Standard Migration Flow

### Phase 1: Assessment
1. Analyze legacy system architecture and code quality
2. Identify business-critical and high-risk components
3. Assess team capabilities and constraints
4. Establish baseline metrics (performance, reliability, maintainability)
5. Document current architecture

### Phase 2: Strategy Definition
1. Define target architecture
2. Choose migration pattern (strangler fig, branch by abstraction, etc.)
3. Identify migration sequence (which components first)
4. Define success criteria for each phase
5. Create rollback strategy

### Phase 3: Migration Pattern Design
1. Design strangler fig interception layer
2. Design anti-corruption layer (if needed)
3. Design data migration strategy
4. Design API coexistence approach
5. Plan testing and validation strategy

### Phase 4: Phased Migration
1. Execute migration in phases
2. Maintain system coexistence
3. Validate feature parity per phase
4. Monitor system health during migration
5. Execute rollback drills

### Phase 5: Decommissioning
1. Verify old system no longer needed
2. Plan data retention and archival
3. Decommission legacy components
4. Update documentation
5. Celebrate milestone

### Phase 6: Continuous Improvement
1. Track post-migration metrics
2. Identify further improvement opportunities
3. Document lessons learned
4. Update modernization playbook

## Output Template

```
1. Legacy System Assessment
2. Target Architecture
3. Migration Strategy
4. Migration Pattern Design
5. Phased Migration Plan
6. Risk Matrix
7. Data Migration Strategy
8. Testing & Validation Plan
9. Rollback Procedures
10. Success Metrics
11. Timeline & Milestones
12. ADRs
```
