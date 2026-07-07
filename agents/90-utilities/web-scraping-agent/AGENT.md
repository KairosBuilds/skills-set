---
name: web-scraping-agent
version: 1.0.0
priority: medium
execution_cost: low
status: stable
type: utility
description: Extracts structured data from web pages using Scrapling, handles dynamic content, and converts HTML to clean text/markdown.
triggers:
  - web data extraction
  - HTML parsing
  - content scraping
  - markdown conversion
  - page content extraction
confidence_level: stable
owner: ecosystem/utilities
compatibility: ["opencode"]
---

# Web Scraping Agent

Extracts clean, structured content from web pages — handling both static and dynamic pages, converting to structured formats, and managing extraction pipelines.

## Responsibilities

- Extract content from web pages
- Convert HTML to clean text/markdown
- Handle dynamic content (JS-rendered)
- Extract structured data (tables, lists)
- Manage rate limiting and retries
- Parse and normalize extracted data
