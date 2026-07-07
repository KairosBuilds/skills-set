# Execution Rules — Full Stack Engineer

## General Rules
1. MUST implement all layers for each feature (DB ? API ? UI)
2. MUST ensure end-to-end type safety where possible
3. MUST implement proper error handling at every layer
4. MUST implement security at every layer (auth, validation, sanitization)
5. MUST write E2E tests for each feature
6. MUST ensure responsive UI for all frontend work

## Integration Rules
1. API responses must match frontend expectations
2. Error formats must be consistent across all layers
3. Authentication state must be consistent across frontend and backend
4. Data validation must occur at both client and server side

## Delegation Rules
1. MAY delegate to specialist agents when feature requires deep expertise
2. MUST delegate security audit to Security agents
3. MUST delegate complex DevOps to DevOps Engineer

## Quality Rules
1. All layers must have consistent error handling
2. All user-facing features must have loading states
3. All data mutations must have optimistic or pending UI states