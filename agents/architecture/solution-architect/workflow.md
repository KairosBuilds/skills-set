# Solution Architect Workflow

## Standard Design Flow

### Phase 1: Requirements Gathering
1. Review functional requirements
2. Identify non-functional requirements (scalability, availability, latency, security, compliance, cost)
3. Clarify constraints (budget, timeline, team expertise, existing infrastructure)
4. Document assumptions

### Phase 2: High-Level Design
1. Identify system boundaries and components
2. Select architecture pattern (monolith, modular monolith, microservices, event-driven, etc.)
3. Design component interactions
4. Create high-level architecture diagram (Mermaid)

### Phase 3: Detailed Design
1. Design component internals
2. Define data flow between components
3. Design API contracts (coarse)
4. Address cross-cutting concerns
5. Create detailed architecture diagrams

### Phase 4: Technology Selection
1. Evaluate technology options per component
2. Apply selection criteria: maturity, community, team expertise, cost, performance
3. Document trade-offs
4. Make recommendations with rationale

### Phase 5: Documentation
1. Write ADRs for each key decision
2. Compile architecture document
3. Include risk assessment and mitigation strategies
4. Add migration/implementation plan

### Phase 6: Review & Validation
1. Present to stakeholders
2. Collect feedback
3. Iterate on design
4. Finalize architecture document

## Output Template

```
1. Executive Summary
2. Requirements (Functional + Non-functional)
3. Architecture Overview (Diagram)
4. Component Details
5. Technology Stack
6. Data Flow
7. Cross-cutting Concerns
8. ADRs
9. Risk Assessment
10. Implementation Roadmap
11. Appendices
```
