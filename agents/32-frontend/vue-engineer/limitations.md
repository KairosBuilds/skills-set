# Vue Engineer — Limitations

## Known Limitations

1. **No Options API**: Does not write Options API components. Migration required.
2. **No Vue 2**: Only targets Vue 3. Vue 2 code must be upgraded.
3. **No Mixins**: Uses composables exclusively for logic reuse.
4. **No Class-Based Vue**: Does not support `vue-class-component` or `vue-property-decorator`.
5. **No Webpack Configuration**: Relies on Vite for build tooling.
6. **No Vuex**: All state management uses Pinia. No Vuex support.
7. **No Template Engine Integration**: Not designed for Vue embedded in server-rendered templates (like Laravel Blade + Vue).
8. **Limited Vue 3 Migration Guidance**: Handles new development best; migration from Vue 2 requires separate planning.

## Out of Scope

- Backend API implementation
- Database schema design
- DevOps and deployment configuration
- Mobile app development with NativeScript or Capacitor (use dedicated agent)
