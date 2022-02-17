### Repository for the project of Kubernetes

This demo project shows a  connection between MongoDB and web application,following Nana Janashia Youtube Tutorial. 
Creating 4 Kubernetes config file such as:

* ConfigMap and Secret to MongoDB
* Deployment and service for MongoDB
* Deployment and service for the Web application with external service

<img width="468" alt="image" src="https://user-images.githubusercontent.com/85910939/154379124-7c3891f9-7fc3-4671-8fd8-a1be1d5e2cbf.png">


#### K8s manifest files 
* mongo-config.yaml
* mongo-secret.yaml
* mongo.yaml
* webapp.yaml

#### K8s commands

##### start Minikube and check status
    minikube start --vm-driver=hyperkit 
    minikube status

##### get minikube node's ip address
    minikube ip

##### get basic info about k8s components
    kubectl get node
    kubectl get pod
    kubectl get svc
    kubectl get all

##### get extended info about components
    kubectl get pod -o wide
    kubectl get node -o wide

##### get detailed info about a specific component
    kubectl describe svc {svc-name}
    kubectl describe pod {pod-name}

##### get application logs
    kubectl logs {pod-name}
    
##### start your Minikube cluster
    minikube start


#### Links
* mongodb image on Docker Hub: https://hub.docker.com/_/mongo
* webapp image on Docker Hub: https://hub.docker.com/repository/docker/nanajanashia/k8s-demo-app
* k8s official documentation: https://kubernetes.io/docs/home/
