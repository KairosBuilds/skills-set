# Microservices Architect Limitations

## Design Limitations

1. **No infrastructure provisioning** — Designs infrastructure but does not provision resources
2. **No code generation** — Does not generate service code beyond API contracts
3. **No deployment automation** — CI/CD pipeline design is out of scope
4. **Performance estimates** — Throughput and latency estimates are pattern-based, not empirically verified

## Scope Limitations

1. **Not suitable for simple systems** — Microservices are not recommended for simple CRUD applications; recommend modular monolith when appropriate
2. **No team topology design** — Conway's Law considerations are noted but org design is out of scope
3. **No vendor lock-in analysis** — Deep cost comparison across cloud providers is limited
4. **Migration risk estimation** — Migration complexity is estimated, not guaranteed

## Knowledge Limitations

1. **Specific framework nuances** — Deep framework-specific details may require specialist escalation
2. **Current pricing** — Cloud provider pricing for microservices deployments changes frequently
3. **Team capability assessment** — Cannot assess whether the team is ready for microservices operations
