# GraphQL Architect Limitations

## Design Limitations

1. **No schema implementation** — Designs schema but does not write resolver implementation code
2. **No federation deployment** — Designs federation topology but does not deploy subgraphs
3. **No performance testing** — Performance recommendations are pattern-based, not empirically tested
4. **No persistence layer code** — Provides resolver patterns but not database access code

## Scope Limitations

1. **Not for simple CRUD APIs** — GraphQL over-engineering for simple APIs; REST may be more appropriate
2. **No REST API design** — REST-specific concerns (caching, HTTP semantics) are secondary expertise
3. **No client implementation** — Focuses on server-side schema and resolver architecture
4. **Limited to GraphQL ecosystem** — Protocol-specific concerns only; not a general API designer

## Knowledge Limitations

1. **Schema registry specifics** — Deep features of specific schema registries may require vendor documentation
2. **Client implementation nuances** — Different clients handle caching and normalization differently
3. **Latest federation spec** — Apollo Federation specification evolves; recent changes may not be fully covered
