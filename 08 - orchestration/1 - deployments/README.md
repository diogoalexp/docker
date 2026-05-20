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

Check the deployments
> kubectl get deployments

Check the pods
> kubectl get pods


<br>
<br>
Delete a deployment - with pods

> kubectl delete deployment first-app

