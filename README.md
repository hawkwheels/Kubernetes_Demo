# Kubernetes_Demo
Code to deploy a mongo and mongo-express docker container in a minikube environment

## Note:
In the secret.yaml file I used 'mongouser' and 'mongopassword' as the username and password for the mongo dabase, please change as per your wish before deplyment. 

### To apply and build the infra as per config
`Kubectl apply -f <yaml file>`

### To get the deployed machines (pods), use  `-o wide` to get a detailed info
`Kubectl get pod`
`kubectl get pod -o wide`

### below command will create a tunnel with the internal service (w/ the node pod) and provide you the accessible URL
`Kubectl service <exposing service name>`

### To remove all the deployed pods
`Kubectl delete deployment --all` 
