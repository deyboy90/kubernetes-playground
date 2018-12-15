### Creating a deployment
kubectl create -f deployment.yaml
kubectl get deployment
kubectl get pods
kubectl describe deployment webapp

*trying to access the http port*
curl localhost:80  # this will fail

### Creating a service to expose the deployment
kubectl create -f service.yaml
kubectl get deployment
kubectl get pods
kubectl describe service webapp-service

*trying to access the http port exposed on the host* 
curl localhost:32000