# Examples

## Create Deployment
```bash
opencode kubernetes-engineer create deployment --name my-app --image my-app:v1
```

## Create Helm Chart
```bash
opencode kubernetes-engineer helm init --name my-app
```

## Configure Network Policies
```bash
opencode kubernetes-engineer network --namespace prod --policy default-deny
```

## Output
Creates Kubernetes manifests and Helm charts for container orchestration.
