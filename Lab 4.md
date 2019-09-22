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


# create psvs
kubectl create -f nfs-0001.yaml
kubectl create -f nfs-0002.yaml
kubectl get pv
kubectl get pvc

