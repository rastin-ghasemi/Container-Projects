In this project, we discuss Kubernetes Architecture
![kubernetes-cluster-architecture](https://github.com/user-attachments/assets/12fb17be-1e2c-40f2-9301-f2d79a0753da)
In the diagram, each node runs the kube-proxy component. You need a network proxy component on each node to ensure that the Service API and associated behaviors are available on your cluster network. However, some network plugins provide their own, third party implementation of proxying. When you use that kind of network plugin, the node does not need to run kube-proxy.

