# How I created the kubernetes-dashboard namespace on my Ubuntu 20.04 app
Finding the kubernetes-dashboard namespace absent in my minikube, I learned I had to create it myself (as opposed to a macOs user who may have it by default) using the following commands: 
```
kubectl create namespace kubernetes-dashboard
kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.0.0/aio/deploy/recommended.yaml
```
First, I created the kubernetes-dashboard namespace. Then I applied the recommended configuration file from the kubernetes github repository.
