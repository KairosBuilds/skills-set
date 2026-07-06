# Examples

## Function too long
```python
# Before: Monolithic function
def process_user(user):
    validate_email(user.email)
    validate_age(user.age)
    user.score = calculate_score(user)
    user.tier = assign_tier(user.score)
    db.save(user)
    send_welcome_email(user.email)
```
