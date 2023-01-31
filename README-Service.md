# Kubernetes Commands - Services

Standard Kubernetes Services related commands with examples.
<br/>

## Service Types

- NodePort
- ClusterIP
- Load Balancer

<br/>

### Node Port

- Maps the internal Port of the Pod to the Kubernete Node in the Cluster.
- Works as a default Load Balancer with the Random assignment algorithm.

<br/>

## Create the Service in the Kubernates Cluster

```sh
kubectl create -f <FILE_NAME>
kubectl create -f definitions/services/nginx-service-nodeport-k8.yaml

# Record the cause of the change in the Kubernetes Cluster
kubectl create -f <FILE_NAME> --record
kubectl create -f definitions/services/nginx-service-nodeport-k8.yaml --record=true
```

<br/>

## View the Service in the Kubernates Cluster

```sh
kubectl get services
kubectl get svc

# Find the URL of the Service
minikube service <SERVICE_NAME>
minikube service nginx-service-nodeport
```

<br/>
<br/>
