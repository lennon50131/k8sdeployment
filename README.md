# k8sdeployment

Using Kubernetes to deploy a mongodb and a web application that is accesible via browser

Whole project will run locally
you will need minikube and docker installed locally
----
install minikube:
macOS: curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-amd64
sudo install minikube-darwin-amd64 /usr/local/bin/minikube

windows: check follow this link https://minikube.sigs.k8s.io/docs/start/
----
install docker:
https://www.docker.com/products/docker-desktop/
----

commands to start >> go to your terminal
  1. minikube start --driver docker
  2. kubectl get node (to check if the cluster is running)
  3. dsd

change directory to where the yaml file is stored then in terminal type the command one by one
  1. kubectl apply -f mongo-config.yaml (this will create the configmap)
  2. kubectl apply -f mongo-secret.yaml (this will create the secret)
  3. kubectl apply -f mongo.yaml (this will create deployment and service)
  4. kubectl apply -f webapp.yaml (this will deploy webapp service)
  5. kubectl get all (this will show all components in the cluster)
  6. minikube service --all (run the application)











