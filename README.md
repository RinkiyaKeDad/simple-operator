## Creating Steps

```
operator-sdk init --domain arshsharma.com --repo github.com/RinkiyaKeDad/simple-operator

operator-sdk create api --group=core --version=v1 --kind=Pod --controller=true --resource=false
```

## Running Steps

```
kind create cluster

make run

kubectl run --image=nginx my-nginx

kubectl annotate pod my-nginx arshsharma.com/add-pod-name-label=true

kubectl get pod my-nginx --show-labels
```