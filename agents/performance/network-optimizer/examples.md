# Examples

## HTTP/2 Server Configuration (Nginx)
```nginx
server {
    listen 443 ssl http2;
    http2_push_preload on;
    
    # Enable brotli compression
    brotli on;
    brotli_types text/plain text/css application/json;
}
```

## Connection Pooling (Node.js)
```typescript
const http2 = require('http2');
const client = http2.connect('https://api.example.com');
// Reuse client for multiple requests
client.request({ ':path': '/users' });
```
