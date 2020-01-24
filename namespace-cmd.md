# K8s-WebForce3

## Namespace
```shell script
k create namespace <namespace> #Nom du namespace
k get namespaces <namespace>

# Create low-ressource-range.yml
k --namespace=<namespace> create -f low-ressource-range.yml

k get LimitRange -A 
#NAMESPACE         NAME                  CREATED AT
#low-usage-limit   low-ressource-range   2020-01-24T11:03:16Z

k -n <namespace> create deployment limited-hog --image vish/stress
k -n <namespace> get pod
k -n <namespace> get pod limited-hog-xxxx -o yaml # Remplacement xxx par uuid pod
k get rs -A

```