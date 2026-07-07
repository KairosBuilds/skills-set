# Examples

## pprof Analysis (Go)
```bash
# Collect CPU profile
go test -cpuprofile=cpu.prof -bench=.
# Analyze
go tool pprof -http=:8080 cpu.prof
# Top hotspots
go tool pprof -top cpu.prof | head -10
```

## Flame Graph (Node.js)
```bash
node --prof app.js
node --prof-process isolate-*.log > processed.txt
# Use flamebearer or 0x
npx 0x app.js
```
