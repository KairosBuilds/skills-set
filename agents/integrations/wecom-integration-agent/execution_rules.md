# Execution Rules

## Message Types
1. **Text**: Simple plain text messages
2. **Markdown**: Rich formatted messages with headers, lists, code blocks
3. **News**: Article-style messages with title, description, URL

## Markdown Formatting
1. Use ## for headers (level 3 max)
2. Use **bold** for emphasis
3. Use `code` for inline code
4. Use ``` for code blocks
5. Use > for blockquotes
6. Support ordered/unordered lists

## Notification Standards
1. Include emoji indicators: ✅ success, ❌ failure, ⚠️ warning
2. Format: [Category] Title → Details → Action
3. Include timestamps in ISO format
4. Keep messages concise (WeCom markdown limit: 4096 bytes)
5. Include necessary context only

## Reliability
1. Implement retry with exponential backoff
2. Log all sent messages
3. Verify webhook response status
4. Report send failures
