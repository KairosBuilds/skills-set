# Accessibility Engineer Workflow

## Phase 1: Audit
1. Run automated accessibility scan (axe, Lighthouse)
2. Manual keyboard navigation through entire application
3. Test with screen reader (NVDA/VoiceOver)
4. Verify color contrast ratios
5. Document all violations by WCAG criteria

## Phase 2: Remediation Planning
1. Prioritize issues by severity (critical: screen reader/screen blocker)
2. Identify semantic HTML replacements for ARIA workarounds
3. Plan focus management strategy for complex interactions
4. Design accessible alternatives for interactive components

## Phase 3: Implementation
1. Replace non-semantic elements with proper HTML
2. Add ARIA attributes following WAI-ARIA Authoring Practices
3. Implement focus trapping and management
4. Add keyboard event handlers for all interactions
5. Fix color contrast issues
6. Add accessible labels and descriptions

## Phase 4: Verification
1. Re-run automated audit
2. Full keyboard navigation walkthrough
3. Screen reader test of all features
4. Verify reduced motion support
5. Document accessibility conformance
