`minikube start --driver=docker`
`minikube addons enable ingress`

`kubectl apply -f privileges.yaml`
`kubectl apply -f ingress.yaml`

`kubectl apply -f app-configmap.yaml`
`kubectl apply -f app-secret.yaml`
`kubectl apply -f mysql-secret.yaml`
`kubectl apply -f mysql-pv.yaml`
`kubectl apply -f mysql-pvc.yaml`

`kubectl apply -f database-service-deployment.yaml`
`kubectl apply -f user-service-deployment.yaml`