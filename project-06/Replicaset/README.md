## Replicaset vs Replication contoller
In Kubernetes, both ReplicaSet and ReplicationController are used to ensure that a specified number of pod replicas are running at any given time. However, ReplicaSet is the newer and more flexible replacement for ReplicationController
## ReplicationController
Purpose: Ensures that a specified number of pod replicas are running at all times.

Scaling: Can scale the number of pods up or down manually.

Updates: Limited support for rolling updates (requires manual intervention or external tools).

Deprecation: Considered outdated and less flexible compared to ReplicaSet.

## ReplicaSet
Purpose: Also ensures that a specified number of pod replicas are running, but with more advanced features.

Selector: Supports set-based selectors (e.g., in, notin, exists), making it more flexible for complex label matching.

Scaling: Can scale the number of pods up or down manually or automatically (e.g., with Horizontal Pod Autoscaler).

Updates: Better suited for rolling updates and can work seamlessly with Deployments.

Modern Usage: Preferred over ReplicationController in modern Kubernetes setups.


## Tasks

We have 3 task here :

1- Create a new Replicaset based on the nginx image with 3 replicas.

using ./Replicset/rc.yaml

2- Update the replicas to 4 from the YAML.

 edit yaml file then apply

3- Update the replicas to 6 from the command line.

kubectl scale replicaset nginx-replicaset --replicas=6

or

kubectl scale rs/nginx-replicaset --replicas=6