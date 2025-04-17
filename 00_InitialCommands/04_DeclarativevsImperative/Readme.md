# Declarative vs Imperative

Let's deploy an Nginx container using both methods.

## Imperative

    kubectl create deployment mynginx1 --image=nginx

## Declarative

    kubectl run redis --image=redis123 --dry-run=client -o yaml > redis-definition.yaml
    kubectl create -f redis-definition.yaml

    kubectl create -f deploy-example.yaml

## Cleanup

    kubectl delete deployment mynginx1
    kubectl delete deploy mynginx2