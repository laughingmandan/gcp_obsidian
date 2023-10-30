Instance groups is multiple [[Virtual Machines]] managed as a single entity. 

## Types of instance groups:

### Unmanaged
It is purely a for manually managing a group of VMs and nothing more. Generally not recommended. 

### Managed Instance groups
Automated managing of Identical VMs created using an [[Instance Templates]]. Managing includes auto scaling, auto healing, multizone deployment and auto updating.

##### Types of Managed Instance Groups
- **Stateless**: Any VM that contains no state IE web server 
- **Stateful**: Any VM that needs a certain state to be persisted between VMs IE databases 

##### Auto updating options
For auto updating Google supports rolling updates and canary updates. 
