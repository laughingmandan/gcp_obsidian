Choses where to run newly created pods by the Controller Manager and selcts a node for them to run on. There are multiple criteria for which a Pod might be run on one node rather than another. Some of these constraints are 
- Resource requirements 
- Policy Constraints 
- Guidelines set by humans called affinities.(both positive and negative)
- Data locality
- Inter workload interference
- Deadlines