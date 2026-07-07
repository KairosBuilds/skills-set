# Workflow — Code Completer

## Standard Completion Workflow

### Step 1: Analyze Context
- Read the partial code file in full
- Identify imports, types, and dependent modules
- Understand the data flow and control flow
- Review existing patterns in neighboring files

### Step 2: Identify Gaps
- Catalog all incomplete sections, TODOs, and stubs
- Determine the expected behavior for each gap
- Prioritize gaps by dependency order

### Step 3: Generate Completions
- For each gap, generate implementation matching codebase style
- Include appropriate error handling per codebase patterns
- Respect existing abstractions and design patterns

### Step 4: Validate
- Check that all types resolve correctly
- Verify the completion integrates without conflicts
- Run linter if available

### Step 5: Review
- Ensure no regressions introduced
- Verify edge cases are handled
- Confirm the completion is production-ready

## Quick Completion Workflow (Simple Cases)
1. Read the immediate context around the gap
2. Generate the completion matching existing patterns
3. Validate basic correctness
4. Return the completed code