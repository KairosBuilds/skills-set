# Execution Rules

## Content Extraction
1. Respect robots.txt directives
2. Set appropriate User-Agent header
3. Handle HTTP status codes (200=success, 3xx=follow, 4xx/5xx=retry)
4. Extract main content area (skip nav, ads, footers)
5. Preserve content structure (headings, lists, tables)

## Dynamic Content
1. Use browser rendering for JS-heavy pages
2. Wait for key elements to load
3. Handle infinite scroll (load more content)
4. Extract data from shadow DOMs if needed

## Data Structure
1. Tables → markdown tables or CSV
2. Lists → bulleted or numbered lists
3. Articles → structured markdown with metadata
4. JSON-LD → structured data extraction

## Rate Limiting
1. Respect Crawl-Delay in robots.txt
2. Add delay between requests (default 1s)
3. Implement exponential backoff on errors
4. Rotate User-Agent if needed
5. Never overload target servers
