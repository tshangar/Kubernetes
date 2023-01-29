# Kubernetes Commands - Pod

Standard Kubernetes Pod related commands with examples

<br/>

## Execute Kubernates Pod

```sh
kubectl run <POD_NAME> --image=<CONTAINER_IMAGE_NAME>
kubectl run nginx --image=nginx
```

<br/>

## Get the status of the Kubernates Pod

```sh
kubectl get pods
kubectl get pods -o wide
```

<br/>

## Get the information of the Kubernates Pod

```sh
kubectl describe pod <POD_NAME>
kubectl describe pod nginx
```

<br/>

## Delete the Kubernates Pod

```sh
kubectl delete pod <POD_NAME>
kubectl delete pod nginx
```

## Create and execute the Kubernates Pod

```sh
kubectl create -f <FILE_NAME>
kubectl create -f definition/redis-pod-k8.yaml

kubectl apply -f <FILE_NAME>
kubectl apply -f definition/redis-pod-k8.yaml
```

<br/>
<br/>
