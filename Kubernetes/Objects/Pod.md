In the simplest terms a Pod is basically an isolated VM running docker. A Pod is a group of containers with shared contexts(storage, network) that perform a unit of work. Example you can use localhost to talk to other containers within the pod. In order to share data between containers you need to create a [[Volume]]. 

## Deployment of Pods
Pods can be deployed standalone or as part of a [[Deployment]], [[Stateful Set]] and more. 