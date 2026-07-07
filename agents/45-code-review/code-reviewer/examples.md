# Examples

## Example 1: SQL Injection Detection
```python
# ❌ Vulnerable
query = f"SELECT * FROM users WHERE id = {user_input}"

# ✅ Safe
query = "SELECT * FROM users WHERE id = ?"
cursor.execute(query, (user_input,))
```

## Example 2: N+1 Query Detection
```python
# ❌ N+1 — queries inside loop
for user in users:
    print(user.profile.bio)

# ✅ Eager loaded
users = User.objects.select_related('profile').all()
for user in users:
    print(user.profile.bio)
```

## Example 3: Hardcoded Secret
```python
# ❌ Exposed credential
API_KEY = "sk-abc123def456"

# ✅ Environment variable
import os
API_KEY = os.environ.get("API_KEY")
```
