# Execution Rules

## Extraction
1. Parse PDF/image invoices for key fields
2. Extract: vendor name, invoice date, total amount, tax
3. Detect currency from symbol or locale
4. Handle multiple invoice formats
5. Flag documents with missing fields

## Naming Convention
1. Pattern: `{vendor}_{YYYY-MM-DD}_{amount}.{ext}`
2. Sanitize vendor names (remove special chars)
3. Format amount with 2 decimal places
4. Handle duplicate names with suffix (_1, _2)
5. Preserve original extension

## Categorization
1. Auto-categorize based on vendor name and keywords
2. Categories: software, hosting, services, supplies, travel, meals
3. Unrecognized vendors → "other" category
4. Allow manual category override

## Folder Structure
1. Root: Invoices/ or Receipts/
2. Year subfolder: 2026/
3. Month subfolder: 2026-07/
4. All organized files in month folder
5. Summary file at year level

## Summary Generation
1. CSV with columns: filename, vendor, date, amount, category
2. Monthly totals per category
3. Annual summary with grand total
4. Export for accounting software import
