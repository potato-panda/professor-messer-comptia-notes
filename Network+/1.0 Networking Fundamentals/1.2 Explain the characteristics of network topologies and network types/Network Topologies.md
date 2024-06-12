---
alias: topology
---
Why?
- useful in planning a new network
	- physical layout of a building or campus
- assist in understanding signal flow
	- troubleshooting problems

# Star
- Hub and Spoke
- used in most large and small networks
- all devices are connected to a central device
- switched Ethernet networks
	- the switch is in the middle
![[star.png]]

# Ring
- used in many popular topologies
	- Token Ring is no longer used
- still used in many Metro Area Networks (MANs) and Wide Area Networks (WANs)
- There are 'Dual-rings'
- Has built-in fault tolerance
	- As in Ring, connection moves circular (e.g. clockwise) so if the ring is cut off somewhere, the connection goes in the opposite direction (counter-clock wise) to reach the destination
![[ring.png]]
# Bus
- were early local area networks
	- uses coaxial cable as the bus
- simple, but prone to errors
	- one break in the link will disable the entire network
- Controller Area Network
	- CAN bus
![[bus.png]]

# Mesh
- multiple links to the same place
	- can be fully or partially connected
- has redundancy, is fault-tolerant, and load balancing
- used in WANs
	- fully mesh and partially meshed
![[mesh.png]]

# Hybrid
- combination of one or more physical topologies
	- most networks are hybrid
![[hybrid.png]]

# Wireless
### Infrastructure
- all devices communicate through access point
- most common wireless communication mode
### Ad hoc networking
- no pre-existing infrastructure
- devices communicate amongst themselves
### Mesh
- ad hoc devices work together to form a mesh 'cloud'
- is self formed and self healing