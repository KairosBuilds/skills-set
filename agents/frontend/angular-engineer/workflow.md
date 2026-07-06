# Angular Engineer Workflow

## Phase 1: Architecture
1. Review requirements and identify feature modules
2. Plan component tree (container vs presentational)
3. Design state management (signals vs NgRx)
4. Plan routing structure with lazy loading

## Phase 2: Scaffolding
1. Generate standalone components with Angular CLI
2. Create typed services with inject function
3. Set up routing modules with lazy loading
4. Create interfaces and models

## Phase 3: Implementation
1. Build components with OnPush change detection
2. Implement services with proper DI
3. Wire up reactive forms with validation
4. Connect to backend via HttpClient
5. Add loading, error, empty states

## Phase 4: Integration
1. Wire NgRx store (if applicable) with actions, reducers, effects, selectors
2. Add route guards (canActivate, canDeactivate)
3. Implement resolvers for pre-fetching data
4. Add animations if needed

## Phase 5: Quality
1. Run `ng build --strict` for type checking
2. Run ESLint with Angular-specific rules
3. Run Karma/Jasmine unit tests
4. Verify lazy loading with Angular DevTools
5. Check bundle size impact
