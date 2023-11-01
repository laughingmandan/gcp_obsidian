Is the part of the [[Node]] that manages the containers within that Node. It is the component that talks to the [[API Server]] in the cluster. This job entails:
- Registering the node to the [[API Server]]
- Responding to health checks from the [[API Server]]
- Making changes to pods requested by the [[API Server]]

## Resources
- https://kubernetes.io/docs/concepts/overview/components/#node-components
- https://kubernetes.io/docs/reference/command-line-tools-reference/kubelet/