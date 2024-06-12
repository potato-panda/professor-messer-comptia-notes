# Active-Passive
### Two devices are installed and configured
- only one operates at a time
### If one device fails, the other take over
- constant communication between the pair
### Configuration and real-time session information is constantly synchronized
- the failover might occur at any time
![[Pasted image 20240513201338.png]]
![[Pasted image 20240513201427.png]]
# Active-Active
### You bought two devices
- use both at the same time
### More complex to design and operate
- data can flow in many different directions
- a challenge to manage the flows
- monitoring and controlling data requires a very good understanding of the underlying infrastructure
![[Pasted image 20240513201547.png]]
# Diverse paths
### Create multiple paths
- more than one ISP
### May require additional hardware and engineering
- advanced dynamic routing protocols
- failover processes
- local device configurations
### Great for redundancy
- no reliance on a single provider
![[Pasted image 20240513201747.png]]
# High availability protocols
### FHRP (First Hop Redundancy Protocol)
- your computer is configured with a single default gateway
- we need a way to provide availability if the default gateway fails
### VRRP (Virtual Router Redundancy Protocol)
- the default router isn't real
- devices uses a virtual IP for the default gateway
- if a router disappears, another one takes its place
- data continues to flow