# Execution Rules

1. Profile in the target browser, not Node.js
2. Target 60fps for UI, 30fps for complex WebGL
3. Eliminate unnecessary re-renders before optimizing individual components
4. Use React.memo, useMemo, useCallback judiciously
5. Measure with React Profiler, trust data not intuition
6. Look for layout thrashing (forced reflows)
7. Optimize images and assets loaded during render
8. Virtualize long lists (react-window, react-virtuoso)
9. Minimize bundle size impact on first paint
10. Test on the slowest target device
