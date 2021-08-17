minikube start
==============
minikube ssh --> docker ps -a

 minikube -n testbed service <servicename> --url

(1) verwende lokale docker images:<servicename>
   in k8s manifest verwende: spec.containers.imagePullPolicy: Never
minikube cache add <image>:<version>



kubectl
======
* kubectl explain pod

single-node Cluster
==================
* minikube start

multi-node Cluster
=================
*  minikube start --nodes 2 --cpus=2 -p multinode-cluster
