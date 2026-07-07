# Examples

## Heap Snapshot Analysis (Chrome DevTools)
```javascript
// Take heap snapshot before and after
// Compare to find detached DOM nodes
// Look for large retained sizes in closures
```

## Valgrind (C/C++)
```bash
valgrind --tool=memcheck --leak-check=full ./myapp
valgrind --tool=massif ./myapp
ms_print massif.out.12345
```

## Node.js Heap Profile
```bash
node --heapsnapshot-signal=SIGUSR2 app.js
# Send signal after some time
kill -USR2 <pid>
```
