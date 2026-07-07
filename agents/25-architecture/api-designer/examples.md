# API Designer Examples

## Example 1: REST API Design

**Request:** "Design a REST API for a blog platform"

**Output:**
- Resources: `/posts`, `/posts/{id}/comments`, `/users/{id}/posts`, `/tags/{slug}/posts`
- Pagination: Cursor-based via `?cursor=xxx&limit=20`
- Response format: Standard envelope with `{ data, meta, errors }`
- Versioning: URL prefix `/v1/`
- Auth: Bearer JWT in Authorization header
- Rate limiting: 1000 requests/hour per API key
- HTTP Status: 200 success, 201 created, 204 deleted, 400 validation, 401 unauthorized, 404 not found, 409 conflict, 422 unprocessable

## Example 2: GraphQL Schema Design

**Request:** "Design a GraphQL API for a social media platform"

**Output:**
```graphql
type Query {
  user(id: ID!): User
  feed(limit: Int, cursor: String): FeedConnection
  search(query: String!, type: SearchType!): SearchResult
}

type Mutation {
  createPost(input: CreatePostInput!): PostMutationResult
  likePost(postId: ID!): LikeMutationResult
  followUser(userId: ID!): FollowMutationResult
}

type Subscription {
  postUpdated(postId: ID!): Post
  userNotifications: Notification
}
```
- DataLoader patterns for batching
- Complexity cost analysis on queries
- Federation-ready for microservices

## Example 3: gRPC Service Design

**Request:** "Design a gRPC API for a real-time chat system"

**Output:**
```protobuf
service ChatService {
  rpc SendMessage(SendMessageRequest) returns (SendMessageResponse);
  rpc ReceiveMessages(ReceiveMessagesRequest) returns (stream Message);
  rpc JoinRoom(JoinRoomRequest) returns (stream RoomEvent);
}
```
- Bidirectional streaming for real-time messaging
- Authentication via interceptor with JWT
- Error handling with standard gRPC codes + rich error details
