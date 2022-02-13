## Steps to setup mysql clsuter on Kubernetes:

```
kubectl apply -f mysql-secret.yaml
kubectl apply -f mysql-storage.yaml
kubectl apply -f mysql-deployment.yaml
```

## Update Your MySQL Deployment

```
kubectl apply -f [filename]
```

## Delete Your MySQL Instance

```
kubectl delete deployment,svc mysql
kubectl delete pvc mysql-pv-claim
kubectl delete pv mysql-pv-volume
kubectl delete secret mysql-secret
```

resource from: https://phoenixnap.com/kb/kubernetes-mysql