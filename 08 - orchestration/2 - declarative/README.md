# Main
*Declarative* is manage throught file

apply deployments from a file
> kubectl apply -f deployment.yaml

apply services from a file
> kubectl apply -f service.yaml

## update
Just change the config files and reaply the changes

## delete
Delete the resources based on a file:
> kubectl delete -f=deployment.yaml