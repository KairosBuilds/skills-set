# Limitations

1. Code splitting increases number of network requests
2. Dynamic imports complicate SSR setups (Next.js, Nuxt)
3. Some libraries cannot be tree-shaken (side effects)
4. Bundle analysis doesn't capture runtime code paths
5. Optimization gains vary by browser (caching, HTTP versions)
6. Reducing bundle size may increase build complexity
7. Cannot optimize server-side bundles the same way
8. Dependency upgrades may reintroduce size regressions
