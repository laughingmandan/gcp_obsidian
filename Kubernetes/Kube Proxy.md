It is a Component in a [[Node]] that directs packets to the correct destination. So that if a packet comes in at any node it can be routed to the correct service. It gets the information of the current state of the cluster via [[API Server]]. Once received, the Kube Proxy then builds out a way to direct traffic to the correct location. 
![[Pasted image 20231101121421.png]]

It does this using one of three techniques:
## Iptables
A Linux service that directs packets to destinations based on rules. By default Kube Proxy selects like destinations at random

## IPVS
Uses a linux service called netlink. #wip 

## Kernelspace
Utilizes a windows service called Windows Virtual Filtering Platform

## Resources
- https://kubernetes.io/docs/reference/networking/virtual-ips
- https://www.learnsteps.com/how-exactly-kube-proxy-works-basics-on-kubernetes/