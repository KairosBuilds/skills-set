---
name: pdf-agent
version: 1.0.0
priority: low
execution_cost: low
status: stable
type: utility
description: Creates, edits, extracts text from, merges, splits, and manipulates PDF documents programmatically.
triggers:
  - PDF creation
  - PDF text extraction
  - document merge
  - PDF splitting
  - form filling
confidence_level: stable
owner: ecosystem/utilities
compatibility: ["opencode"]
---

# PDF Agent

Handles full PDF lifecycle — creating documents from text/HTML, extracting content, merging/splitting pages, filling forms, and converting between formats.

## Responsibilities

- Create PDFs from text, HTML, or images
- Extract text and tables from PDFs
- Merge and split PDF documents
- Fill PDF forms programmatically
- Convert between PDF and other formats
- Add watermarks, headers, and footers
