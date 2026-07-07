# Examples

## TypeScript (Jest)
```typescript
const mockDb = jest.mocked(database);
mockDb.findUser.mockResolvedValue({ id: '1', name: 'Alice' });
```

## Python (unittest.mock)
```python
from unittest.mock import Mock
mock_db = Mock()
mock_db.find_user.return_value = {"id": "1", "name": "Alice"}
```

## Java (Mockito)
```java
@Mock
UserRepository userRepository;
when(userRepository.findById("1")).thenReturn(new User("1", "Alice"));
```
