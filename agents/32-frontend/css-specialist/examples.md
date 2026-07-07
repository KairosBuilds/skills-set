# CSS Specialist Examples

## Example 1: Tailwind Design System Configuration

```javascript
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      colors: { brand: { 50: '#f0f9ff', 500: '#3b82f6', 900: '#1e3a5f' } },
      spacing: { 18: '4.5rem', 88: '22rem' },
      fontFamily: { sans: ['Inter', 'system-ui', 'sans-serif'] }
    }
  }
};
```

## Example 2: Responsive Card Component with Tailwind

```html
<div class="mx-auto max-w-sm rounded-xl border border-gray-200 bg-white p-6 shadow-sm transition-shadow hover:shadow-md dark:border-gray-700 dark:bg-gray-800">
  <h3 class="text-lg font-semibold text-gray-900 dark:text-gray-100">Title</h3>
  <p class="mt-2 text-sm text-gray-600 dark:text-gray-400">Content here.</p>
</div>
```

## Example 3: SCSS with CSS Grid

```scss
// _grid.scss
@use 'variables' as *;

.card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: $spacing-6;

  @media (max-width: 640px) {
    grid-template-columns: 1fr;
  }
}
```
