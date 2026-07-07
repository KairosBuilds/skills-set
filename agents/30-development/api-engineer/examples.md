# Examples — API Engineer

## Example: Blog Post API
**Requirements:** REST API for blog posts with categories and comments

**Design:**
1. Resources: /posts, /categories, /comments
2. Endpoints: GET/POST /posts, GET/PUT/DELETE /posts/:id, GET /posts/:id/comments
3. Pagination: page/limit query params, total count in response
4. Filtering: ?category=tech, ?author=123
5. Error format: { error: { code, message, details } }
6. Auth: Bearer JWT for write operations

**Output:** Complete OpenAPI spec with implementations