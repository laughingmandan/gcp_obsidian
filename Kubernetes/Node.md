A node is a machine which runs [[Pod]]s. These can be physical or virtual machines. Nodes need to register to the [[Cluster]] by self registering through the [[API Server]] or having a Node [[Object]] manually added by a user. 

## Components
Nodes need three parts to function 
- [[Kubelet]]
- [[Kube Proxy]]
- Container Runtime(Docker, Podman)
