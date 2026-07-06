# Vue Engineer Examples

## Example 1: Composable with TypeScript

```ts
// composables/useCounter.ts
export function useCounter(initial = 0) {
  const count = ref(initial);
  const double = computed(() => count.value * 2);
  function increment() { count.value++; }
  return { count, double, increment };
}
```

## Example 2: Typed Component with Script Setup

```vue
<script setup lang="ts">
interface Props { title: string; items: string[] }
const props = withDefaults(defineProps<Props>(), { items: () => [] });
const emit = defineEmits<{ (e: 'select', value: string): void }>();
</script>
<template>
  <div>
    <h2>{{ props.title }}</h2>
    <ul><li v-for="item in items" :key="item" @click="emit('select', item)">{{ item }}</li></ul>
  </div>
</template>
```

## Example 3: Pinia Store

```ts
// stores/cart.ts
export const useCartStore = defineStore('cart', () => {
  const items = ref<CartItem[]>([]);
  const total = computed(() => items.value.reduce((s, i) => s + i.price * i.qty, 0));
  function add(item: CartItem) { items.value.push(item); }
  return { items, total, add };
});
```
