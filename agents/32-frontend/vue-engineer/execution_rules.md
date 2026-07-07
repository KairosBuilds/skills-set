# Execution Rules for Vue Engineer Agent

## Core Rules

1. **Composition API Only**: Use `<script setup>` syntax. Never use Options API.
2. **TypeScript**: All components typed with `<script setup lang="ts">`. Define interfaces for props and emits.
3. **Pinia for State**: Use Pinia stores for shared state. Avoid provide/inject for complex state.
4. **Performance**: Use `v-memo` for large lists. Lazy load routes with `defineAsyncComponent`.
5. **Template Simplicity**: Keep template logic minimal. Use computed properties instead of complex expressions in templates.
6. **Accessibility**: Semantic HTML, ARIA attributes, keyboard navigation.
7. **CSS Scoping**: Use `<style scoped>` by default. Use CSS modules or global styles intentionally.
8. **Component Organization**: One component per file. Use composables for reusable logic.
9. **Props Definition**: Define props with type and default values using `withDefaults(defineProps<Props>(), defaults)`.
10. **Emits Typing**: Define emits with `defineEmits<{ (e: 'event', payload: Type): void }>()`.

## Prohibited

- Options API (`data()`, `methods`, `computed` as object)
- Mixins (use composables instead)
- `this` access in `<script setup>` blocks
- Direct DOM manipulation
- Inline styles without scoped CSS

## Enforcement

Run `vue-tsc --noEmit` for type checking and `eslint` with Vue 3 recommended rules before completing tasks.
