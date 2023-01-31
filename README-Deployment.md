# Kubernetes Commands - Deployments

Standard Kubernetes Deployments related commands with examples

<br/>

## Create the Deployments in the Kubernates Cluster

```sh
kubectl create -f <FILE_NAME>
kubectl create -f definitions/deployments/nginx-deployment-k8.yaml

# Record the cause of the change in the Kubernetes Cluster
kubectl create -f <FILE_NAME> --record
kubectl create -f definitions/deployments/nginx-deployment-k8.yaml --record=true
```

<br/>

## View the Deployments in the Kubernates Cluster

```sh
kubectl get deployments
```

<br/>

## View all the Kubernetes Objects in the Kubernates Cluster

```sh
kubectl get all
```

<br/>

## Update to existing Deployment in the Kubernates Cluster

```sh
# Update the definition file with differnt Container version and execute the below command.
# Default behaviour is Rolling Update.
kubectl apply -f <FILE_NAME>
kubectl apply -f definitions/deployments/nginx-deployment-k8.yaml

# Below command will not update the original deployment definition file.
kubectl set image deployment/<DEPLOYMENT_NAME> <CONTAINER>=<CONTAINER>:<NEW_TAG>
kubectl set image deployment/nginx-deployment nginx=nginx:1.9.1
```

<br/>

## View the description of the Deployment in the Kubernates Cluster

```sh
kubectl describe deployment <DEPLOYMENT_NAME>
kubectl describe deployment nginx-deployment
```

<br/>

## Rollback the Deployment in the Kubernates Cluster

```sh
kubectl rollout undo deployment/<DEPLOYMENT_NAME>
kubectl rollout undo deployment/nginx-deployment
```

<br/>

## Delete the Deployment in the Kubernates Cluster

```sh
# This command will also delete all the underlying Pods
kubectl delete deployment <DEPLOYMENT_NAME>
kubectl delete deployment nginx-deployment
```

<br/>

## View the status of the Deployment in the Kubernates Cluster

```sh
kubectl rollout status deployment/<DEPLOYMENT_NAME>
kubectl rollout status deployment/nginx-deployment
```

<br/>

## View the history of the single Deployment in the Kubernates Cluster

```sh
kubectl rollout history deployment/<DEPLOYMENT_NAME>
kubectl rollout history deployment/nginx-deployment
```

<br/>
<br/>
