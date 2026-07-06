# Vue Engineer — Supported Frameworks

| Framework | Version | Status | Notes |
|---|---|---|---|
| Vue | 3.4+ | Primary | Composition API with `<script setup>` |
| Nuxt | 3.12+ | Primary | SSR, SSG, file-based routing, auto-imports |
| Pinia | 2.1+ | Primary | State management with Composition API |
| Vue Router | 4.3+ | Supported | Client-side routing |
| Vite | 5.x | Tooling | Dev server and build |
| Vitest | 1.x | Testing | Unit and component testing |
| VueUse | 10.x | Utilities | Composition API utilities library |

## Framework-Specific Rules

- **Nuxt**: Use `useFetch`, `useAsyncData` for data fetching; auto-import composables; `definePageMeta` for route metadata
- **Pinia**: Define stores with setup syntax (function form), not options form
- **Vue Router**: Lazy load routes with dynamic imports
