# Deployments

Let's now use the Deployment template instead of the Pod template.
## Give you details about the deployments
    kubectl explain deployment | head -n3

## Create the Deployment

    kubectl apply -f deploy-example.yaml

## Get the pods list

    kubectl get pods -o wide
    
## Describe the pod

    kubectl describe pod deploy-example

## Get the Deployment info

    kubectl get deploy
    kubectl describe deploy deploy-example

## Get the ReplicaSet name

    kubectl get rs

## Describe the ReplicaSet

    kubectl describe rs

## Cleanup

    kubectl delete -f deploy-example.yaml