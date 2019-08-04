# Dockers-Kubernetes-Demo



# 1.] Dockers Demo:

![Architecture](https://github.com/sriram5795/Dockers-Kubernetes-Demo/blob/master/Architecture.PNG)

  ### Creating an Image:
```
  $ docker build -t angular .

  $ docker build -t nodejs .

  $ docker build -t springboot .
```
  ### Creating a new image with new tag to PUSH:
```
  $ docker tag springboot sriram5795/docker-demo-springboot

  $ docker tag nodejs-service sriram5795/docker-demo-nodejs

  $ docker tag angular sriram5795/angular
```
  ### Loging into dockerhub to push the image:
```
  $ docker login
```
  ### Push the image:
```
  $ docker push sriram5795/docker-demo-springboot

  $ docker push sriram5795/docker-demo-nodejs

  $ docker push sriram5795/docker-demo-angular
```
  ### To Stop and remove all containers:
```
  $ docker stop $(docker ps -a -q)

  $ docker rm $(docker ps -a -q)
```
  ### Creating a network:
```
  $ docker network create -d bridge mynetwork
```
  ### Creating a Volume:
```
  $ docker volume create my-redis-data

  $ docker volume inspect  my-redis-data
```

  ### Running a container:
```
  $ docker run -d -v  my-redis-data:/data --name redis --network mynetwork redis:alpine

  $ docker run -d -v  my-redis-data:/data --name redis -p 6379:6379 redis:alpine --appendonly yes

  $ docker run -d --name nodejs --network mynetwork sriram5795/docker-demo-nodejs

  $ docker run -d --name springboot --network mynetwork sriram5795/docker-demo-springboot

  $ docker run -d -p 8080:80 --name angular --network mynetwork sriram5795/docker-demo-angular

  $ docker run -d -p 3001:3000 --name nodejs --network mynetwork nodejs-service 

  $ docker run -d -p 8081:8080 --name springboot --network mynetwork springboot
```
  ### Execute commands in conatiner:
  #### For Slim
```
  $ docker exec -it container_id /bin/bash
```
  #### For alpine
```
  $ docker exec -it container_id /bin/ash
```
