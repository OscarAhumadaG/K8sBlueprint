# ReplicaSet

Let's now use the ReplicaSet template instead of the Pod template.

## Give you details about the replicaset

    kubectl explain replicaset | grep VERSION

## Create the ReplicaSet

    kubectl apply -f rs-example.yaml

## Get the pods list

    kubectl get pods -o wide

## Get the ReplicaSet name

    kubectl get rs

## Describe the ReplicaSet

    kubectl describe rs rs-example

## Scale a ReplicaSet

    kubectl scale rs new-replica-set --replicas=5

## Edit a ReplicaSet

    kubectl edit replicaset new-replica-set

## Edit a ReplicaSet
    kubectl edit replicaset new-replica-set

## Cleanup

    kubectl delete -f rs-example.yaml