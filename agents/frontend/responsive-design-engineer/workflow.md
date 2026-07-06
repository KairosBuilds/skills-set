# Responsive Design Engineer Workflow

## Phase 1: Planning
1. Review design mockups for all breakpoints
2. Identify layout shifts between breakpoints
3. Plan grid or flex layouts per section
4. Determine component-level container query needs

## Phase 2: Implementation
1. Build base mobile layout first
2. Add responsive utilities progressively (`sm:`, `md:`, `lg:`, `xl:`)
3. Implement CSS Grid with `auto-fit`/`auto-fill` for flexible grids
4. Apply container queries for reusable components
5. Set up fluid typography with `clamp()`

## Phase 3: Enhancement
1. Add responsive navigation (hamburger menu, etc.)
2. Implement responsive images with `srcset`
3. Optimize touch targets for mobile
4. Add responsive tables with horizontal scroll
5. Ensure forms are mobile-friendly (input zoom, button sizing)

## Phase 4: Verification
1. Test at 320px, 375px, 640px, 768px, 1024px, 1280px, 1440px+
2. Test with real mobile device if available
3. Verify no horizontal scroll
4. Check all interactive elements are reachable
5. Verify font sizes remain readable at all breakpoints
