# Examples

## Example 1: Create PDF from Markdown
```
Input: "Create PDF from README.md"
Actions:
1. Convert markdown to HTML
2. Style with CSS (headers, code blocks, tables)
3. Generate PDF with table of contents
4. Add page numbers
5. Output: README.pdf (12 pages)
```

## Example 2: Merge Documents
```
Input: "Merge 3 PDF reports into one"
Actions:
1. Load report-q1.pdf (15 pages)
2. Load report-q2.pdf (18 pages)
3. Load report-q3.pdf (14 pages)
4. Merge preserving order
5. Add cover page with title
6. Output: annual-report.pdf (47 pages)
```

## Example 3: Form Filling
```
Input: "Fill W-9 tax form with company info"
Actions:
1. Load W-9.pdf (fillable form)
2. Map fields: name, business, address, TIN
3. Fill form fields
4. Flatten form (prevent edits)
5. Output: filled-w9.pdf
```
