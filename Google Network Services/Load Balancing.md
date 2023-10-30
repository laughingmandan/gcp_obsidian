A way to distribute traffic hitting one IP across multiple instances of the same application. It can be both **External** and **Internal** to GCP. You can also use multiple types of load balancers for the same application. Ex. you have an external application load balancer balancing traffic going into [[Instance Groups]] across multiple regions. Within each region is an instance group with an internal load balancer balancing traffic to all [[Virtual Machines]] within that instance group. See below what that might look like.

![[Pasted image 20231018130815.png]]

## Types of load balancers

#### Application Load Balancers
Distributes HTTP(S) across Google Compute Engine([[Instance Groups]], [[Virtual Machines]]) Google Kubernetes Engine, Cloud Run, and external applications outside of Google Cloud. 

#### Network Load Balancers
Operate on lower level protocols such as TCP and UDP. There are two types of network load balancers: 
- **Proxy**: hides the backend details and takes a performance hit. Use for slower protocols like TCP. 
- **Passthrough**: just does the balancing and no other function. Use for time critical applications like game servers, voice chat. 

**Network Protocol Types supported:** 
- TCP
- UDP
- ESP
- GRE
- ICMP
- ICMPv6

## Security
Having a load balancer can help increase security. Every type of load balancer can provide DDoS protection. While only application and network proxy load balancers can provide [[Cloud Armor]]

## Service Tiers 
Certain load balancers can have multiple tiers. 
- **Premium**: Traffic travels on google networks. Use when you need high performance low latency
- **Standard**: Traffic travels on regular ISP networks. Use when cost is more important.

## Resources
- https://cloud.google.com/load-balancing/docs/choosing-load-balancer
- https://cloud.google.com/load-balancing/docs/passthrough-network-load-balancer
- https://cloud.google.com/load-balancing/docs/choosing-load-balancer#summary-gclb