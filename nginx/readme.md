```
yum install git
git clone https://github.com/punitporwal07/ingressController.git
cd nginx/
kubectl apply -f ns-sa.yaml
kubectl apply -f default-server-secret.yaml
kubectl apply -f nginx-configmap.yaml
kubectl apply -f custom-resource-definitions.yaml
kubectl apply -f rbac.yaml
kubectl apply -f nginx-ingress-daemonset.yaml
```
```
kubectl get pods -n nginx-ingress
kubectl logs nginx-ingress-15pod-nam3 -n nginx-ingress
```
