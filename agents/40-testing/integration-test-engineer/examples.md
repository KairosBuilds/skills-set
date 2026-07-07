# Examples

## TypeScript (Jest + Testcontainers)
```typescript
describe('UserRepository integration', () => {
  let container: PostgreSqlContainer;

  beforeAll(async () => {
    container = await new PostgreSqlContainer().start();
  });

  it('persists and retrieves a user', async () => {
    const repo = new UserRepository(container.getConnectionUri());
    await repo.save({ id: '1', name: 'Alice' });
    const user = await repo.findById('1');
    expect(user.name).toBe('Alice');
  });
});
```

## Python (Pytest + Testcontainers)
```python
def test_user_repository(postgres_container):
    uri = postgres_container.get_connection_url()
    repo = UserRepository(uri)
    repo.save(User(id="1", name="Alice"))
    user = repo.find_by_id("1")
    assert user.name == "Alice"
```
