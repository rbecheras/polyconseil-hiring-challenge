# Polyconseil challenge

> deploy a wordpress on k8s

## using minikube

Requirement: git, docker-ce, kubectl, minikube

```
$ sudo minikube start --vm-driver=none
$ git clone git@github.com:rbecheras/polyconseil-hiring-challenge.git
$ cd polyconseil-hiring-challenge
$ kubectl apply -k .
$ echo Application deployed at $(sudo minikube service wordpress --url)
```