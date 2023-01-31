# Kubernetes Commands - ReplicaSet

Standard Kubernetes ReplicaSet related commands with examples

<br/>

## Create the ReplicaSet in the Kubernates Cluster

```sh
kubectl create -f <FILE_NAME>
kubectl create -f definitions/replicaset/nginx-deployment-k8.yaml
```

<br/>

## View the ReplicaSet in the Kubernates Cluster

```sh
kubectl get replicaset
```

<br/>

## Update replication count in the ReplicaSet

```sh
# Update the ReplicaSet definion file with the new Replicas count and execute the below command.
kubectl replace -f <FILE_NAME>
kubectl replace -f definitions/replicaset/nginx-deployment-k8.yaml

# Use the below kubectl scale command with scale option. This command will not update the definition file.
kubectl scale --replicas=<NEW_COUNT> -f <FILE_NAME>
kubectl scale --replicas=6 -f definitions/replicaset/nginx-deployment-k8.yaml

# Use the below kubectl scale command with scale option. This command will not update the definition file.
kubectl scale --replicas=<NEW_COUNT> <TYPE> <REPLICA_SET_METADATA_NAME>
kubectl scale --replicas=6 replicaset nginx-replica-set
```

<br/>

## Edit the current running definition file of the ReplicaSet in the Kubernates Cluster

```sh
# This command will not update the original definition file.
kubectl edit replicaset <REPLICA_SET_METADATA_NAME>
kubectl edit replicaset nginx-replica-set
```

## Delete the ReplicaSet in the Kubernates Cluster

```sh
# This command will also delete all the underlying Pods
kubectl delete replicaset <REPLICA_SET_METADATA_NAME>
kubectl delete replicaset nginx-replica-set
```

<br/>
<br/>
