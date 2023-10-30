It is a container that sees the current state of the cluster and in a feedback loop fashion makes changes so that the current state is moving towards the desired state. It does this by most often sending messages to the [[API Server]] to receive the current and desired state. Then it makes more calls to the [[API Server]] to create or destroy nodes and pods to move towards the desired state. There are multiple feedback loops inside this a list of which can be found in the link to the github repo. The most notable ones are:
- [[Node Controller]]
- [[Job Controller]]
- [[Endpoints Slice Controller]]
- [[Service Account Controllers]]


## Resources
- https://kubernetes.io/docs/concepts/architecture/controller/
- https://github.com/kubernetes/kubernetes/tree/master/pkg/controller
- https://kubernetes.io/docs/concepts/overview/components/#kube-scheduler