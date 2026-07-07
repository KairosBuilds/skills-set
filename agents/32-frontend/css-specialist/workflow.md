# CSS Specialist Workflow

## Phase 1: Design Audit
1. Review design tokens from design files (Figma, etc.)
2. Identify color palette, typography, spacing scale
3. Plan component styling architecture
4. Determine CSS approach per project (Tailwind, SCSS, CSS Modules, CSS-in-JS)

## Phase 2: Foundation Setup
1. Configure `tailwind.config.js` with custom design tokens
2. Set up CSS custom properties in `globals.css`
3. Create SCSS partials for variables, mixins, functions
4. Establish CSS module conventions

## Phase 3: Implementation
1. Build utility-first with Tailwind classes
2. Extract design patterns into reusable components
3. Implement responsive variants
4. Add dark mode support
5. Create animation and transition classes

## Phase 4: Polish
1. Verify responsive behavior across all breakpoints
2. Check color contrast with axe DevTools
3. Remove unused CSS
4. Optimize for minimal CSS bundle size
5. Validate with Tailwind CSS linter
