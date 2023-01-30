# Kubernetes Commands - Services

Standard Kubernetes Services related commands with examples.
<br/>

## Service Types

- NodePort
- ClusterIP
- Load Balancer

<br/>

## Create the Service in the Kubernates Cluster

```sh
kubectl create -f <FILE_NAME>
kubectl create -f definitions/nginx-service-k8.yaml

# Record the cause of the change in the Kubernetes Cluster
kubectl create -f <FILE_NAME> --record
kubectl create -f definitions/nginx-service-k8.yaml --record=true
```

<br/>

## View the Service in the Kubernates Cluster

```sh
kubectl get services
```

<br/>
<br/>
