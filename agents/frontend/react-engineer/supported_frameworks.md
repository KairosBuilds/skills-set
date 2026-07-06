# React Engineer — Supported Frameworks

| Framework | Version | Status | Notes |
|---|---|---|---|
| React | 18.x – 19.x | Primary | Server Components, hooks, Suspense |
| Next.js | 14+ | Primary | App Router, RSC, Server Actions |
| Remix | 2.x | Supported | Nested routes, loaders, actions |
| Vite | 5.x | Tooling | Dev server and build tool |
| TanStack Router | 1.x | Supported | Type-safe routing |
| Storybook | 8.x | Optional | Component development and documentation |

## Framework-Specific Rules

- **Next.js**: Default to App Router; use `'use client'` sparingly
- **Remix**: Use loader/action pattern for data; prefer form mutations
- **Vite**: Configure path aliases in `vite.config.ts`
