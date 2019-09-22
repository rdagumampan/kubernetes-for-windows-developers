Service types:
- cluster ip
- node port
- load balancer
- external name

Different ports in service under load balancer
- IP
- Load Balancer Ingress
- Port
- Target Port
- Node Port
- Endpoints

kube ctl get ing
kubectl get pods --selector="name=bad-frontend"
kubectl get deployment,svc,pods,pvc

# create psvs
kubectl create -f nfs-0001.yaml
kubectl create -f nfs-0002.yaml
kubectl get pv
kubectl get pvc

# working with secrets
kubectl create -f secret.yaml
kubectrl get secrets

# secrets via env
kubectl create -f secret-via-env.yaml
kubectl exec -it secret-env-pod env | grep SECRET_
kubectl get pods

# secrets via volume
kubectl create -f secret-via-pod.yaml
kubectl exec -it secret-vol-pod ls /etc/secret-volume
kubectl exec -it secret-vol-pod cat /etc/secret-volume/username
kubectl exec -it secret-vol-pod cat /etc/secret-volume/password
