ETCD is a key value store for desired and current state of the cluster. This includes:
## Information stored 

##### Cluster State
This is the current state of everything within the cluster. ex. pods, services, endpoints, nodes, secrets and more. 

##### API Data
Any information taken in by the [[API Server]] is stored within ETCD. This includes many configurations. 

##### Meta Data
Any data that helps uniquely identify an [[Object]]. This includes labels, name UID, and namespace. 

##### Service Discovery Data
Information that allows discovery between containers, end users, and workloads.