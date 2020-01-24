# k8s-webforce3

## Check
```shell script
  kubectl get nodes
  kubectl get node
  kubectl get node -o wide
```

## Deployment example
```shell script
  kubectl create deployment nginx --image=nginx
  kubectl get deployments
  kubectl describe deployment nginx
  kubectl get events
  kubectl get deployment nginx -o yaml 
  kubectl get deployment nginx -o yaml > first.yaml
  kubectl get deployment two --image=nginx --dry-run -o yaml
  kubectl create deployment nginx --export -o yaml
  kubectl get deployment nginx --export -o json
  kubectl get svc nginx
```
## CPU and limits
```shell script

```