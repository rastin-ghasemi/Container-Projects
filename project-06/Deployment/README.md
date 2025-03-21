## Key Features of a Deployment
1- Declarative Updates:

You define the desired state in a YAML file, and Kubernetes handles the details of achieving and maintaining that state.

2- Scaling:

You can easily scale the number of Pods up or down by updating the replicas field in the Deployment.

3- Rolling Updates:

Deployments support rolling updates, allowing you to update your application with zero downtime by gradually replacing old Pods with new ones.

4- Rollback:

If an update fails or causes issues, you can roll back to a previous version of the Deployment.

5- Self-Healing:

If a Pod crashes or is deleted, the Deployment ensures that the desired number of replicas is maintained.

6- Pod Template:

Deployments use a Pod template to define the specifications of the Pods it manages (e.g., container image, labels, environment variables, etc.).

## Create a deployment named nginx that runs the nginx image with 3 replicas

kubectl apply -f deployment.yaml