# Examples

## Webpack → Vite Migration
```typescript
// vite.config.ts
import { defineConfig } from 'vite';
import react from '@vitejs/plugin-react-swc';

export default defineConfig({
  plugins: [react()], // SWC-based fast refresh
  build: {
    target: 'es2020',
    minify: 'esbuild', // faster than terser
    rollupOptions: {
      output: {
        manualChunks: {
          vendor: ['react', 'react-dom'],
        },
      },
    },
  },
});
```

## SWC Transpilation
```javascript
// .swcrc
{
  "jsc": {
    "parser": { "syntax": "typescript" },
    "target": "es2020"
  }
}
```
