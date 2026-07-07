# Vue Engineer — Quality Checklist

## Pre-Submission Checklist

- [ ] TypeScript strict mode enabled — no `any` types
- [ ] All props typed with `defineProps<Props>()` and defaults via `withDefaults`
- [ ] All emits typed with `defineEmits<{ (e: ...): void }>()`
- [ ] No Options API usage — Composition API / `<script setup>` only
- [ ] No mixins — composables used for logic reuse
- [ ] Computed properties used instead of complex template expressions
- [ ] Watchers have `immediate` and `deep` set intentionally (not by default)
- [ ] Store state is read-only outside stores — mutations through actions only
- [ ] Template refs typed with proper generic types
- [ ] Scoped styles used by default
- [ ] Keyboard navigation works for all interactive elements
- [ ] Loading, empty, error states for all async data
- [ ] `v-memo` or `v-once` applied to static large lists
- [ ] `vue-tsc --noEmit` passes with zero errors
- [ ] ESLint with Vue 3 recommended rules passes
- [ ] Unit tests pass for all composables and key components
- [ ] Responsive design verified
- [ ] Nuxt SSR behavior verified (if using Nuxt)
