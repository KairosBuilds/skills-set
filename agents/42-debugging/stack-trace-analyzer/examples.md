# Stack Trace Analyzer — Examples

## Example 1: Java NullPointerException
**Input:**
```
Exception in thread "main" java.lang.NullPointerException
    at com.myapp.service.UserService.getProfile(UserService.java:42)
    at com.myapp.controller.UserController.showProfile(UserController.java:15)
    at com.myapp.Main.main(Main.java:8)
```
**Analysis:** Root cause at `UserService.java:42` — `user.getAddress()` called on null user object retrieved from database.

## Example 2: Python Traceback
**Input:**
```
Traceback (most recent call last):
  File "app.py", line 25, in <module>
    result = divide(10, 0)
  File "utils.py", line 5, in divide
    return a / b
ZeroDivisionError: division by zero
```
**Analysis:** Root cause at `app.py:25` — calling `divide` with divisor 0 without validation.

## Example 3: JavaScript Async Stack
**Input:**
```
TypeError: Cannot read properties of null (reading 'id')
    at processOrder (orders.js:42)
    at async handleCheckout (checkout.js:18)
```
**Analysis:** Root cause at `orders.js:42` — `order.items` is null. Missing null check after API response.
