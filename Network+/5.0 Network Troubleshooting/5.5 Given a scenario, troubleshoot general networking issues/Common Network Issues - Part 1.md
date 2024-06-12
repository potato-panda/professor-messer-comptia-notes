# Half-duplex Ethernet
### If two devices communicate simultaneously, you have a collision
# Collisions
### On a half-duplex link, collisions are normal
- heavy utilization can cause excessive collisions
### Most Ethernet connections are full-duplex
- where are the collisions coming from?
### Interface configuration issues
- duplex mismatch
### Hardware issue
- could indicate a bad NIC or bad driver
![[Pasted image 20240516161613.png]]
	- runts
	- giants
	- input errors
	- CRC
	- collisions
	- interface resets
	- late collisions
# Broadcast storms
### Some processes use broadcasts to communicate
- send a message to every device
### Broadcast domain
- a single VLAN
- broadcast domains are separated by routers
### Large number of broadcasts can impact performance
- each device must process every broadcast
# Troubleshooting broadcast storms
### Packet capture
- identify the source
### Research the process that's broadcasting
- there may be another option
### Separate the network into smaller broadcast domains
- change one large subnet into many smaller routed subnets
![[Pasted image 20240516161827.png]]
# Duplicate MAC addresses
### Not a common occurrence
- MAC addresses are designed to be unique
- may be an on-path attack
### Mistake can happen
- locally administered MAC addresses
- manufacturing error
### Intermittent connectivity
- confirm with a packet capture, should see ARP contention
### Use the ARP command from another computer
- confirm the MAC matches the IP
# Duplicate IP addresses
### Static address assignments
- must be very organization
### DHCP isn't a panacea
- Static IP addressing
- Multiple DHCP servers overlap
- Rogue DHCP servers
### Intermittent connectivity
- two addresses "fight" with each other
### Blocked by the OS
- checks when it starts
# Troubleshooting duplicate IP addresses
### Check your IP addressing
- did you misconfigure?
### Ping an IP address before static addressing
- does it respond?
### Determine the IP address
- ping the IP address, check the ARP table
- find the MAC address in your switch MAC table
### Capture the DHCP process
- what DHCP servers are responding
# Multicast flooding
### Multicast
- used for one-to-many traffic flows
- for example, live video feeds
### Switches forward multicast traffic
- there's no multicast destination address in the switch forwarding table
- all multicast traffic is sent to every switch port
- multicast flooding
### Every device receives the multicast traffic
- consumes resources on the remote device
- uses bandwidth and switch processing time
# IGMP snooping
### IGMP (Internet Group Management Protocol)
- hosts and routers use IGMP to direct multicast transmissions
### Switches can watch for these IGMP messages
- the switch then intelligently forwards multicasts to those specific devices
- Enable IGMP Snooping
![[Pasted image 20240516163532.png]]
# Asymmetric routes
### Traffic follows one path on egress
- and a different path on ingress, or vice versa
- this is often by design
### This can be difficult to troubleshoot
- it may be challenging to understand the path
### Firewalls may drop sessions
- an unexpected traffic flow is dropped by default
### Traceroute can help
- identify potential asymmetric routes
![[Pasted image 20240516164347.png]]
# Switching loops
### A fear of every network administrator
- Spanning Tree Protocol is often configured
### Switches communicate by MAC address
- every device has it's own address
- every packet is directed
### Broadcast and multicasts are sent to all
- broadcast repeated to all switch ports
### Nothing at the MAC address level to identify loops
- IP has TTL (Time to Live)
# (No) loop
https://youtu.be/XfvBsCcJ500?si=fCiCe0cHDTg_g1MR&t=671
# Routing loops
### Router A thinks the next hop is to Router B
- Router B thinks the next hop is to router A
- and repeat until TTL is 0
### Easy to misconfigure
- especially with static routing
### A traceroute will tell the story
- check the routing tables in each L3 device
- modify the routing tables as needed
![[Pasted image 20240516165715.png]]
![[Pasted image 20240516165708.png]]
# Missing route
### A route to the destination network does not exist
- the packet will be dropped
### ICMP host unreachable message will be sent to the source address
- source device will be informed of the error
### Check your routes
- in both directions
![[Pasted image 20240516165903.png]]