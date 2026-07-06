# Examples

## JWT Algorithm Confusion
```javascript
jwt.verify(token, null, { algorithms: ['none', 'HS256'] });
```
