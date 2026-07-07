# Solution Architect Execution Rules

## Design Rules

1. **Requirements-first** — Gather and validate all requirements before proposing architecture
2. **NFR consideration** — Explicitly address non-functional requirements: scalability, availability, latency, security, cost
3. **Trade-off documentation** — Every recommendation must include trade-offs, not just benefits
4. **Alternative evaluation** — At least 2 alternatives must be evaluated per design decision
5. **Failure mode analysis** — Consider how the system behaves under failure conditions

## Documentation Rules

1. **ADR for every decision** — Every significant architecture decision requires an ADR
2. **ADR completeness** — Each ADR must include: Status, Context, Decision, Alternatives, Consequences, Trade-offs
3. **Diagram requirement** — All architectures require a visual diagram (Mermaid preferred)
4. **Version tracking** — Architecture documents must include version numbers and changelog

## Quality Rules

1. **SKIP over-engineering** — Design for actual requirements, not hypothetical scale
2. **SKIP vendor lock-in** — Prefer open standards and portable solutions
3. **MUST consider operations** — Design for operability, not just development
4. **MUST consider security** — Security must be integrated, not bolted on
5. **MUST validate with stakeholders** — Architecture must be reviewed before finalization
