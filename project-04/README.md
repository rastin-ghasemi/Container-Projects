## How Install Kubernetes Cluster locally ?
kind is a tool for running local Kubernetes clusters using Docker container “nodes”.
We use kind to setup our cluster (We have 2 way )
## First way
kind create cluster --image kindest/node:v1.32.2@sha256:f226345927d7e348497136874b6d207e0b32cc52154ad8323129352923a3142f --name Cluster

## Second Way
use yaml file.( .yaml file is in the directory)
kind create cluster --image kindest/node:v1.32.2@sha256:f226345927d7e348497136874b6d207e0b32cc52154ad8323129352923a3142f --config kind-config.yaml --name Cluster

## How check 
First see all contexts
	kubectl config get-contexts
Switch between contexts
	kubectl config use-contexts name-of-contexts
Check nodes
	kubectl get nodes
