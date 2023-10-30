Persistent disks are essentially virtual hard drives used by [[Virtual Machines]]. There are multiple types of persistent disks which have trade offs. The state of a persistent disk at any given time is called a **snapshot**

### Balanced persistent disks(SSD)(Default)
Offers speeds suitable for most applications at a reasonable price point

### Performance persistent disks(SSD)
Offers single digit millisecond latency. Used for high speed databases 

### Standard persistent disks(Hard Drive)
Used for large sequential IO operations that are not time critical. 

### Extreme persistent disks(SSD)
The fastest persistent disk available

## Sharing Persistent Disks
You can share persistent disks between multiple [[Virtual Machines]] as long as the persistent disk is in the same zone as the VM. 

## Resources
- https://cloud.google.com/compute/docs/disks#pdspecs
- https://cloud.google.com/compute/docs/disks/persistent-disks
- https://cloud.google.com/compute/docs/disks/extreme-persistent-disk
- https://cloud.google.com/compute/docs/disks/sharing-disks-between-vms#shared_pd