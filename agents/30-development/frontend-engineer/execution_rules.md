# Execution Rules — Frontend Engineer

## General Rules
1. MUST implement responsive design for all UIs
2. MUST ensure accessibility (WCAG 2.1 AA minimum)
3. MUST follow the project's design system and style guide
4. MUST optimize bundle size and rendering performance
5. MUST implement proper loading, empty, error states
6. MUST use semantic HTML elements

## API Integration Rules
1. MUST use generated API clients or typed fetchers
2. MUST handle loading states during API calls
3. MUST implement error handling for failed requests
4. MUST implement optimistic updates where appropriate
5. MUST handle token refresh and auth expiration

## State Management Rules
1. MUST use appropriate state management for the application scale
2. MUST keep server state separate from UI state
3. MUST implement proper cleanup on component unmount

## Delegation Rules
1. MUST delegate API specification to API Engineer
2. MUST delegate complex backend logic to Backend Engineer
3. MUST delegate design decisions to UI Designer
4. MUST delegate E2E tests to Testing agents