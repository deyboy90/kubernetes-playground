## Types of services

#### ClusterIP
This is the default type of service in Kubernetes. It is used to allocate an internal cluster IP 

```
kubectl apply -f cluster-ip.yaml
kubectl get svc
kubectl describe svc/webapp-service
```
TargetPort is the Port which the application is configured to listen on. Port is how the application will be accessed from the outside.

#### NodePort

Exposes the service on each Node’s IP at a static port (the NodePort). A ClusterIP service, to which the NodePort service will route, is automatically created. The service can be accessed from outside the cluster NodeIP:NodePort

TargetPort is the Port which the application is configured to listen on. Port is how the application will be accessed from the outside.

```
kubectl apply -f nodeport.yaml
kubectl get svc
kubectl describe svc/webapp-service
```

`curl localhost:30000` 
