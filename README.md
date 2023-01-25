# Kubernetes

## Kubernetes Commands

Standard Kubernetes commands with examples

<br/>

### Execute Kubernates POD

```sh
kubectl run <POD_NAME> --image=<CONTAINER_IMAGE_NAME>
kubectl run nginx --image=nginx
```

<br/>

### Get the status of the Kubernates POD

```sh
kubectl get pods
kubectl get pods -o wide
```

<br/>

### Get the information of the Kubernates POD

```sh
kubectl describe pod <POD_NAME>
kubectl describe pod nginx
```

<br/>
<br/>
