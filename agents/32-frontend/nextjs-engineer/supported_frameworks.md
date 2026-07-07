# Next.js Engineer — Supported Frameworks

| Framework | Version | Status | Notes |
|---|---|---|---|
| Next.js | 14+ | Primary | App Router, Server Actions |
| React | 18+ | Core | Server Components, hooks |
| Tailwind CSS | 3.x | Styling | Utility-first CSS |
| Prisma | 5.x | Data | ORM for Server Components |
| Drizzle ORM | 0.30+ | Data | Type-safe SQL ORM |
| NextAuth.js | 5.x | Auth | Authentication integration |
| tRPC | 11.x | API | Type-safe API layer |
| TanStack Query | 5.x | Client | Client-side data fetching |

## Framework-Specific Rules

- **Next.js**: `next.config.js` with proper image domains, redirects, headers
- **Prisma/Drizzle**: Server-only imports (use `server-only` package)
- **NextAuth**: Route handler for `[...nextauth]`; middleware for session
