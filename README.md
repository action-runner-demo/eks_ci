# eks_ci
eks with github action runner demo

```bash
kubectl create ns github-runner-ysg-debug
kubectl create secret generic gh-pat -n github-runner-ysg-debug --from-literal=pat=$GITHUB_PAT
kubectl apply -f self-hosted-runner
```