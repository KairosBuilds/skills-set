# Examples

## Dynamic Import (Code Splitting)
```typescript
const Dashboard = lazy(() => import('./Dashboard'));
const AdminPanel = lazy(() => import('./AdminPanel'));

<Suspense fallback={<Loading />}>
  <Routes>
    <Route path="/dashboard" element={<Dashboard />} />
    <Route path="/admin" element={<AdminPanel />} />
  </Routes>
</Suspense>
```

## Bundle Analyzer (Webpack)
```javascript
// webpack.config.js
const BundleAnalyzerPlugin = require('webpack-bundle-analyzer').BundleAnalyzerPlugin;
module.exports = {
  plugins: [new BundleAnalyzerPlugin()],
};
```
