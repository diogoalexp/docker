# Main
Start a cluster
> minikube start --driver=docker

Check the cluster status
> minikube status

Tag local container with the hub respository name
> docker tag kub-first-app diogopereiraezo/kub-first-app

Push to hub repository
> docker push diogopereiraezo/kub-first-app

Create a deployment object
> kubectl create deployment first-app --image=diogopereiraezo/kub-first-app

Create a service throught the expose deployment
> kubectl expose deployment first-app --type=LoadBalancer --port=8080

## Aux commands

Check the services
> kubectl get services

Check the deployments
> kubectl get deployments

Check the pods
> kubectl get pods

Check the minikube exposed addresses
> minikube service first-app

## Scale

Scale Up
> kubectl scale deployment/first-app replicas=3

Scale Up
> kubectl scale deployment/first-app replicas=1

## Update

Update image - you must define a new tag to let kubets know there is a change

> kubectl set image deployment/first-app kub-first-app=diogopereiraezo/kub-first-app:2

> kubectl rollout status deployment/first-app

## Delete

Delete a deployment - with pods

> kubectl delete deployment first-app

