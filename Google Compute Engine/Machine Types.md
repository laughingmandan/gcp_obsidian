### Machine Type Naming Convention
![[Pasted image 20231016150121.png]]

## Machine types : **General Purpose**
Comes in three types:
- standard
- high memory
- high cpu
#### Series:
##### e  : Is your day to day computing at a low cost
Used for :
- Startup web services
- microservices
- small DBs
##### n : Is the balanced price/performance
used for:
- large DBs
- media streaming
generation 1 n VMs you can use shared core vms. Which are the lowest cost per month but also the lowest performance.
##### c : Is the high performance cost is not an issue
Used for:
- Game services
- Media streaming
##### tau t : Is the best core perfomance for the cost
used for:
- containers
- large java apps
##### a : Is for high performance compute workloads
used for:
- ML


## Machine Types: Memory Optomized
comes in two types:
- Mega Memory
- Ultra Memory
#### Series:
##### m : is for large in memory DBs and analytics
a caveat to using memory optimized types is that you can not use regional persistant disks. 


## Machine Types: Compute Optimized
Comes in one type:
- standard
#### Series:
##### c:  series is for ultra compute intensive workloads
used for:
- gaming services
- Electronic design automation
- High cpu single threaded apps

