# Vue Engineer — Supported Languages

| Language | Proficiency | Notes |
|---|---|---|
| TypeScript | Primary | All Vue SFCs use `<script setup lang="ts">` |
| JavaScript | Supported | ES2023+, Composition API |
| CSS/SCSS | Styling | Scoped styles with `<style scoped>` |
| HTML | Template | Vue template syntax |
| Pug | Optional | Alternative template syntax |

## Language Conventions

- TypeScript for all new components and composables
- Avoid Options API JavaScript — Composition API in TypeScript is default
- PascalCase for component filenames (e.g., `UserProfile.vue`)
- camelCase for composable functions (e.g., `useUserAuth.ts`)
