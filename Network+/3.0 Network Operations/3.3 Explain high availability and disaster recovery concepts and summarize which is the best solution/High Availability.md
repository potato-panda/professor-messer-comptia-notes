# Fault Tolerance
### Maintain uptime in the case of failure
- if a problem occurs, what happens?
- can degrade performance
### Fault tolerance add complexity
- the cost of managing the environment increases
### Single device fault tolerance
- RAID, redundant power supplies, redundant NICs
### Multiple device fault tolerance
- server farms with load balancing
- multiple network paths
# Redundancy and fault tolerance
### Redundant hardware components
- multiple devices, load balancing power supplies
### RAID
- Redundant Array of Independent Disks
### Uninterruptible power supplies 9UPS)
- prepare for the disconnections
### Clustering
- a logical collective of servers
### Load balancing
- shared service load across components
# Building fault tolerant networks
![[Pasted image 20240513195037.png]]
![[Pasted image 20240513195047.png]]
![[Pasted image 20240513195118.png]]
![[Pasted image 20240513195037.png]]
# High availability
### Redundancy doesn't always mean always available
- may need to be enabled manually
### HA (high availability)
- always on, always available
### May include many different components working together
- watch for single points of failure
### Higher availability almost always means higher costs
- there's always another contingency you could add
- upgraded power, high-quality server components, etc
# Load balancing
### Some servers are active
- others are on standby
### If an active server fails, the passive server takes it's place
![[Pasted image 20240513195348.png]]
![[Pasted image 20240513195445.png]]
![[Pasted image 20240513195501.png]]
# Building HA networks
![[Pasted image 20240513195519.png]]
![[Pasted image 20240513195526.png]]
![[Pasted image 20240513195533.png]]
![[Pasted image 20240513195603.png]]
# NIC teaming
### Load Balancing / Fail Over (LBFO)
- aggregate bandwidth, redundant paths
- becomes more important in the virtual world
### Multiple network adapters
- looks like a single adapter
- integrate with switches
### NICs talk to each other
- usually multicast instead of broadcast
- fails over when a NIC doesn't respond
# Port Aggregation
![[Pasted image 20240513195831.png]]
# Multipathing
![[Pasted image 20240513195857.png]]