### Useful Commands

```
## Start minikube cluster with Docker and check status
$ minikube start --driver=docker
$ minikube status

## List all running pods
$ kubectl get pods -A
$ kubectl get pods --all-namespaces

## Show cluster nodes
$ kubectl get nodes

## See if the cluster is running
$ minikube status

## Open Kubernetes Dashboard UI
$ minikube dashboard

## Stop the cluster
$ minikube stop

## Delete the cluster
$ minikube delete
```

---

##### get minikube node's ip address
    minikube ip

##### get basic info about k8s components
    kubectl get node
    kubectl get pod
    kubectl get svc
    kubectl get all
    kubectl get configmap
    kubectl get secret

##### get extended info about components
    kubectl get pod -o wide
    kubectl get node -o wide

##### get detailed info about a specific component
    kubectl describe svc {svc-name}
    kubectl describe pod {pod-name}

##### get application logs
    kubectl logs {pod-name}
    
##### stop your Minikube cluster
    minikube stop

<br />

> :warning: **Known issue - Minikube IP not accessible** 

If you can't access the NodePort service webapp with `MinikubeIP:NodePort`, execute the following command:
    
    minikube service webapp-service

---

### Links
* mongodb image on Docker Hub: https://hub.docker.com/_/mongo
* webapp image on Docker Hub: https://hub.docker.com/repository/docker/nanajanashia/k8s-demo-app
* k8s official documentation: https://kubernetes.io/docs/home/
