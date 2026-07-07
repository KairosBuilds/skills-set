# Examples

## Example 1: Article Extraction
```
Input: "Extract blog post content from URL"
URL: https://example.com/blog/post-title
Actions:
1. Fetch page (200 OK)
2. Parse HTML (article tag found)
3. Extract: title, author, date, body
4. Clean HTML: remove scripts, ads, nav
5. Convert to markdown
6. Output: clean markdown with frontmatter
```

## Example 2: Table Extraction
```
Input: "Extract pricing table"
URL: https://example.com/pricing
Actions:
1. Fetch page (200 OK)
2. Find table element (3 rows, 5 cols)
3. Extract header row
4. Extract data rows
5. Format as markdown table
6. Output: structured table data
```

## Example 3: Dynamic Content
```
Input: "Extract content from SPA page"
URL: https://example.com/spa-page
Actions:
1. Launch headless browser
2. Wait for .content selector (5s)
3. Extract rendered HTML
4. Convert to markdown
5. Close browser
6. Output: complete content
```
