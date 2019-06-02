To Deploy:

```
kubectl apply -f es-cluster-ds.yaml

kubectl apply -f es-cluster-svc.yaml
kubectl rollout status -f es-cluster-svc.yaml

kubectl apply -f es-cluster-sts.yaml
kubectl rollout status -f es-cluster-sts.yaml

```