# Delete minikube
`minikube delete`
# Start minikube on docker
`minikube start --driver=docker`

# Enable NGINX Ingress on minikube
`minikube addons enable ingress`

## Use following commands for basic configuration 

## User `minikube kubectl --` if `kubectl` not working or not found

`kubectl apply -f privileges.yaml`

`kubectl apply -f ingress.yaml`

`kubectl apply -f app-configmap.yaml`
`kubectl apply -f app-secret.yaml`
`kubectl apply -f mysql-secret.yaml`
`kubectl apply -f mysql-persistence-volume.yaml`
`kubectl apply -f mysql-persistence-volume-clame.yaml`
`kubectl apply -f database-service-deployment.yaml`

## In product service api we need ADMIN role to add data

## `sudo nano /etc/hosts` to edit domain proxy
## Add `192.168.49.2 microservice.test` in hosts file
## check ADDRESS and HOSTS of ingress `kubectl get ingress`