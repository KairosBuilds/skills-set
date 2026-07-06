# Examples — Library Engineer

## Example: Date Utility Library
**Requirements:** Lightweight date formatting and manipulation library

**API Design:**
- formatDate(date, format) -> string
- parseDate(str, format) -> Date
- addDays(date, n) -> Date
- differenceInDays(a, b) -> number
- isWeekend(date) -> boolean

**Implementation (TypeScript):**
1. Tree-shakeable exports
2. Full TypeScript types
3. Runtime validation
4. Zero dependencies
5. ESM and CJS support

**Output:** Published npm package with docs and tests