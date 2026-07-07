# GraphQL Architect Examples

## Example 1: Federation Architecture

**Request:** "Design a federated GraphQL architecture for our microservices"

**Output:**
- Subgraphs: Accounts (users, auth), Products (catalog, inventory), Orders (checkout, history), Reviews (ratings, feedback)
- Supergraph: Apollo Gateway composing all subgraphs
- Entity keys: User { id }, Product { id, sku }, Order { id }
- Reference resolvers: Order.user -> Accounts, Order.items -> Products
- Federation version: Apollo Federation 2.x
- Gateway: Apollo Router (Rust) for production, Apollo Gateway (Node.js) for development

## Example 2: Schema Design for CMS

**Request:** "Design a GraphQL schema for a headless CMS"

**Output:**
```graphql
type Query {
  post(id: ID!): Post
  posts(filter: PostFilter, pagination: PaginationInput): PostConnection!
  category(slug: String!): Category
  search(query: String!, pagination: PaginationInput): SearchResultConnection!
}

type Mutation {
  createPost(input: CreatePostInput!): PostMutationResult!
  updatePost(id: ID!, input: UpdatePostInput!): PostMutationResult!
  deletePost(id: ID!): DeleteResult!
  addComment(postId: ID!, content: String!): CommentMutationResult!
}

type Post implements Node {
  id: ID!
  title: String!
  slug: String!
  content: String!
  excerpt: String
  author: User!
  categories: [Category!]!
  tags: [Tag!]!
  comments: CommentConnection!
  createdAt: DateTime!
  updatedAt: DateTime!
}
```
- DataLoader for categories, tags, comments per post
- Complexity scoring: post.comments weighted higher than post.title
- Auth directives: @auth(requires: ADMIN) on mutations

## Example 3: Performance Optimization

**Request:** "Our GraphQL queries are slow (2-5s). Optimize."

**Findings:**
- Issue: No DataLoader - N+1 queries on all relationship lookups
- Issue: Query depth up to 12 levels allowing expensive nested queries
- Issue: No persisted queries
- Resolution: Implement DataLoader (200ms → 30ms), depth limit to 7, implement persisted queries for common queries
- Result: p95 latency reduced from 3s to 120ms
