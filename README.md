# eks_ci
eks with github action runner demo

```bash
kubectl create ns github-runner
kubectl create secret generic gh-pat -n github-runner --from-literal=pat=$GITHUB_PAT
kubectl apply -f self-hosted-runner
```