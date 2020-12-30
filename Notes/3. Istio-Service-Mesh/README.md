# Running A Service Mesh With Istio (Envoy):
## STEP-1:
- Run the following three YAML Files to setup istio in **istio-system namespace**:
    - 1-istio-init.yaml
    - 2-istio-minikube.yaml          
    - 3-kiali-secret.yaml
    
## STEP-2:
- Add the following label to the namespace for automatic sidecar(envoy) injection:
```kubectl label ns default  istio-injection=enabled```

## STEP-3:
- Run all the **application related YAML** files in kubernetes directory as usual in the order mentioned in [README.md](https://github.com/sriram-ponangi/Dockers-Kubernetes-Demo/tree/master/Notes/2.%20Kubernetes)


## STEP-4:
- Look at the NodePort services in **istio-system** namesapce for port number of other applications like Kiali, Grafana, etc.
- The actual application will run as usual in **default** namespace but with two containers due to the istio sidecar pod injector.
