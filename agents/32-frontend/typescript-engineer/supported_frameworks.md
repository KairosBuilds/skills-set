# TypeScript Engineer — Supported Frameworks

| Framework | Version | Status | Notes |
|---|---|---|---|
| TypeScript | 5.5+ | Primary | The language itself |
| ts-pattern | 5.x | Supported | Pattern matching library |
| zod | 3.x | Supported | Runtime type validation |
| tRPC | 11.x | Supported | End-to-end type safety |
| Prisma | 5.x | Supported | Generated types from schema |
| TanStack Query | 5.x | Supported | Generic query/mutation types |

## Framework-Specific Rules

- **tRPC**: Ensure proper procedure types; infer client types from server
- **Prisma**: Use generated `Prisma` namespace types; create DTO types separate from Prisma types
- **Zod**: Infer TypeScript types from zod schemas with `z.infer<typeof schema>`
