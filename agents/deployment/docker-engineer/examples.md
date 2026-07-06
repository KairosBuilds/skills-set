# Examples

## Create Dockerfile
```bash
opencode docker-engineer init --runtime node:20-alpine --port 3000
```

## Create Docker Compose
```bash
opencode docker-engineer compose --services web,db,redis
```

## Optimize Image
```bash
opencode docker-engineer optimize --dockerfile ./Dockerfile
```

## Output
Creates optimized Dockerfiles and Docker Compose configurations for application containerization.
