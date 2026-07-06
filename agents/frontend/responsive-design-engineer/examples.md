# Responsive Design Engineer Examples

## Example 1: Responsive Grid with Auto-Fill

```html
<div class="grid grid-cols-1 gap-4 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4">
  <div class="card" v-for="item in items">{{ item }}</div>
</div>
```

## Example 2: Container Query Component

```css
.card-container { container-type: inline-size; }
@container (min-width: 400px) {
  .card { display: flex; gap: 1rem; }
  .card-image { width: 200px; }
}
```

## Example 3: Fluid Typography

```css
:root {
  --font-size-h1: clamp(1.75rem, 4vw + 1rem, 3rem);
  --font-size-body: clamp(0.875rem, 1vw + 0.5rem, 1.125rem);
  --spacing-section: clamp(2rem, 5vw, 6rem);
}
```
