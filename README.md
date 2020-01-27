## Cheat Sheet

- Autocomplete kubectl
```
source <(kubectl completion bash)
```
or
```
source <(kubectl completion zsh)
```
- Generate deployment
```
kubectl run [deployment-name] --image=[image-name]] --dry-run -oyaml
```
- Generate pods
```
kubectl run [pods-name] --image=[image-name] --generator=run-pod/v1 --dry-run -oyaml
```

- Generate Service
```
kubectl expose pod front-end-pod --dry-run -o yaml
```
- Cheat from help '-h'
```
kubectl expose -h | grep "# " -A2
kubectl create -h | grep "# " -A2
kubectl run -h | grep "# " -A2
```