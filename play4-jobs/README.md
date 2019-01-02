### Creating a job
```
kubectl apply -f job-primes.yml
kubectl get jobs
kubectl get pods
kubectl describe deployment primes
```

```
kubectl apply -f job-primes-parallel.yml
kubectl get jobs
kubectl get pods
kubectl describe deployment primes-parallel
```


Reference Links:
https://supergiant.io/blog/making-sense-of-kubernetes-jobs/
