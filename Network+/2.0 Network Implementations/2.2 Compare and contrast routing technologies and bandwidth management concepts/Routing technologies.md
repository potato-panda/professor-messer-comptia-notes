# Routing tables
### A list of directions for your packets
- table with many routes to your destination
- packets stop at every router and ask for directions
### Routing table in routers, workstations, and other devices
- every devices need directions
# The hop
### A hop
- a packet passes through a router
### The next hop
- the destination address of the next gateway
### A router doesn't need to know how to get everywhere
- it just needs to know how to get out of here
- a default route handles everything not specifically listed
### There is "TTL" in IPv4, "hop limit" in IPv6
- avoids packet loop forever
# Configuring the next hop
### Every router needs to know where traffic should be sent
- your packet is always asking for directions
### A router with the incorrect next hope will result in a routing problem
- data will go in the wrong direction
- a routing loop is easy to create
	- you'll know quickly if there's a loop
# Default routes
### A route when no other route matches
- the "gateway of last resort"
### A remote site may have only one route
- go that way => rest of the world
- destination of 0.0.0.0/0
### Can dramatically simplify the routing process
- works in conjunction with all other routing methods
# Routing metrics
### Each routing protocol has it's own way of calculating the best route
- i.e. RIPv2, OSPF, EIGRP
### Metric values are assigned by the routing protocol
- RIPv2 metrics aren't useful to OSPF or EIGRP
### Use metric to choose between redundant links
- choose the lowest metric,
- i.e. 1 is better than 2
# Administrative distances
### What if you have two routing protocols, and both know about a route to a subnet?
- two routing protocols, two completely different metric calculations
- you can't compare metrics across routing protocols
- which one do you choose?
### Administrative distances
- used by the router to determine which routing protocol has priority
![[Pasted image 20240510164356.png]]
# Managing network utilization
### Many different devices
- desktop, laptop, VoIP phones, mobile devices
### Many different applications
- mission critical applications, streaming video, streaming audio
### Different apps have a different network requirements
- voice is real-time
- recorded streaming video has a buffer
- database applications is interactive
### Some applications are "more important" than others
- voice traffic must have priority over YouTube
# Traffic shaping
### Traffic shaping, packet shaping
### Control by bandwidth usage or data rates
### Set important applications to have high priorities than other apps
### Manage the Quality of Service (QoS)
- Routers, switches, firewalls, QoS devices
![[Pasted image 20240510164748.png]]
