# 1.] Kubernetes Demo:

![Architecture](https://github.com/sriram5795/Dockers-Kubernetes-Demo/blob/master/Notes/2.%20Kubernetes/Architecture.PNG)

## Creating Volumes on Host Machine:
### 1. Creating Persistent Volumes:
```
kubectl create -f redis-pv.yml
```

### 2. Creating Persistent Volume Claim:
```
kubectl create -f redis-pv.yml
```

## Creating Deployments and Services:
```
kubectl create -f redis-deployment.yml
kubectl create -f redis-service.yml

kubectl create -f springboot-deployment.yml
kubectl create -f springboot-service.yml

kubectl create -f nodejs-deployment.yml
kubectl create -f nodejs-service.yml

kubectl create -f angular-deployments.yml
kubectl create -f angular-service.yml
```

## Creating NodePort(LoadBalancer) Services for nodejs and springboot microservices:
```
kubectl create -f ./nodePort-services/nodejs-service.yml
kubectl create -f ./nodePort-services/springboot-service.yml
```



## To Delete All Services or Deployments:
```
kubectl delete --all services
kubectl delete --all deployments
```



## Tip: To Create all the Deployments/Services/PV/PVC with a single command use:
```
kubectl create -f .
```
