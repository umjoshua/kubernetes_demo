# kubernetes_demo
This is a kubernetes demo application that connects mongodb and mongo express on Minikube.

## How to run
1. Create the secret
```sh
$ kubectl apply -f secret.yaml
```
2. Create the ConfigMap
```sh
$ kubectl apply -f configMap.yaml
```
3. Create the mongo deployment and mongodb-service
```sh
$ kubectl apply -f mongo.yaml
```
4. Create the mongo express deployment and load balancer service
```sh
$ kubectl apply -f mongo-express.yaml
```