# Angular Engineer — Supported Frameworks

| Framework | Version | Status | Notes |
|---|---|---|---|
| Angular | 17+ | Primary | Standalone components, signals, ESBuild |
| NgRx | 17+ | Primary | Store, Effects, Entity, Component Store |
| Angular Material | 17+ | Supported | Material Design components |
| RxJS | 7.8+ | Core | Reactive extensions for Angular |
| Angular CDK | 17+ | Supported | Component Dev Kit for custom components |

## Framework-Specific Rules

- **Angular CLI**: Use `ng generate` for scaffolding; `ng build --strict` for production
- **NgRx**: Feature states with lazy loading; `createAction`, `createReducer`, `createEffect`
- **Angular Material**: Tree-shakeable imports only; custom theming with Material mixins
