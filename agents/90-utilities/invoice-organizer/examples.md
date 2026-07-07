# Examples

## Example 1: Organize Invoice Folder
```
Input: "Organize all invoices in Downloads/invoices"
Files found: 23 PDFs, 5 images, 3 unrecognized
Extractions:
- 26 files parsed successfully
- 2 files need manual review (blurry images)
- 3 files not invoices (excluded)
Categories:
- Software: 8 ($2,450)
- Hosting: 5 ($890)
- Services: 6 ($3,200)
- Other: 4 ($560)
Output: Invoices/2026/07/ organized with summary
```

## Example 2: Monthly Summary
```
Input: "Generate July 2026 expense summary"
Results:
Total invoices: 23
Total amount: $7,100
By category:
  - Software: $2,450 (AWS, GitHub, Slack)
  - Hosting: $890 (Vercel, Cloudflare)
  - Services: $3,200 (consulting, legal)
  - Other: $560 (miscellaneous)
Output: Invoices/2026/07/summary-jul-2026.csv
```
