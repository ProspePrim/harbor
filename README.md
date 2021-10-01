Harbor

```
kubectl create ns harbor

helm -n harbor upgrade --install harbor --set expose.ingress.hosts.core= \  # harbor domain
  --set expose.ingress.hosts.notary=  \  # notary domain
  --set harborAdminPassword: "" . # admin pass

```
