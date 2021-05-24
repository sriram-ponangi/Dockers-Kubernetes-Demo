# Dockers-Kubernetes-Serverless-Demo

### [Notes:](https://github.com/sriram-ponangi/Dockers-Kubernetes-Demo/tree/master/Notes)
  - [X] **[Dockers](https://github.com/sriram-ponangi/Dockers-Kubernetes-Demo/tree/master/Notes/1.%20Dockers)**
    - Breif explanation of the overall architecture and the list of commands to deploy the application containers.
    - Applications Used:
      - **[Backend / Microservices:](https://github.com/sriram-ponangi/dockers-k8s-demo-microservices)** Springboot and Node.js Applications
      - **[Frontend:](https://github.com/sriram-ponangi/dockers-k8s-demo-frontend)** Angular Application
      - **[Data Store:](https://hub.docker.com/_/redis)** Redis Container
      
  - [X] **[Kubernetes](https://github.com/sriram-ponangi/Dockers-Kubernetes-Demo/tree/master/Notes/2.%20Kubernetes)**
    - Breif explanation of the overall architecture and YAML manifest files to run the kubernetes objects.
      - Commands to deploy the pods, services, persistent volumes, etc.    
      - [X] **[Service Mesh (Kubernetes + Istio + Envoy)](https://github.com/sriram-ponangi/Dockers-Kubernetes-Demo/tree/master/Notes/3.%20Istio-Service-Mesh)**
        - YAML Manifest files for Istio components as kubernetes objects and other monitoring tools like Kiali, Grafana, etc.
        - Commands to deploy the pods, services, persistent volumes, etc. as ServiceMesh with Envoy as sidecar.
    - Applications Used:
      - **[Backend / Microservices:](https://github.com/sriram-ponangi/dockers-k8s-demo-microservices)** Springboot and Node.js Applications
      - **[Frontend:](https://github.com/sriram-ponangi/dockers-k8s-demo-frontend)** Angular Application
      - **[Data Store:](https://hub.docker.com/_/redis)** Redis Container 

 - [ ] **Serverless - In-progress**
     - Breif explanation of the overall architecture and AWS lambda functions code.
     - Applications Used:
        -  **[Backend / Microservices:]()** AWS Lambda Functions and API Gateway
        -  **[Frontend:](https://github.com/sriram-ponangi/dockers-k8s-demo-frontend)** Angular Application deployed in S3 with CloudFront
        -  **[Data Store:](https://aws.amazon.com/dynamodb/)** AWS DynamoDB
 

