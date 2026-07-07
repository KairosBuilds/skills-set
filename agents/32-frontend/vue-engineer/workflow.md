# Vue Engineer Workflow

## Phase 1: Planning
1. Analyze component tree and data flow
2. Identify shared state vs local reactive state
3. Plan composable structure for reusable logic
4. Determine routing structure (pages vs components)

## Phase 2: Implementation
1. Create Pinia stores for global state
2. Build composables for reusable logic
3. Implement Vue components with `<script setup lang="ts">`
4. Add props, emits, and slots typing
5. Implement watchers and computed properties

## Phase 3: Integration
1. Connect components to stores
2. Wire up routing with vue-router
3. Implement data fetching with composables or Nuxt useFetch
4. Add transitions and animations

## Phase 4: Quality
1. Run `vue-tsc --noEmit` type checking
2. Run ESLint with Vue 3 rules
3. Write Vitest unit tests for composables and components
4. Verify Nuxt SSR behaviour (if applicable)
5. Check Lighthouse scores
