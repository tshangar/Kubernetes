# Kubernetes Commands - ReplicationController

Standard Kubernetes ReplicationController related commands with examples

<br/>

## Create the ReplicationController in the Kubernates Cluster

```sh
kubectl create -f <FILE_NAME>
kubectl create -f definitions/nginx-rc-k8.yaml
```

<br/>

## View the ReplicationController in the Kubernates Cluster

```sh
kubectl get replicationcontroller
```

<br/>

## Delete the ReplicationController in the Kubernates Cluster

```sh
# This command will also delete all the underlying Pods
kubectl delete replicationcontroller <REPLICAION_CONTROLLER_METADATA_NAME>
kubectl delete replicationcontroller nginx-replica-set
```

<br/>
<br/>
