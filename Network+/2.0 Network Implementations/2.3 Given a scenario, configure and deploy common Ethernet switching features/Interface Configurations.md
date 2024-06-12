# Basic interface configuration
### Speed and duplex
- speed: 10/100/1000/10 Gig
- Duplex: Half/Full
- Automatic and manual
- Needs to match on both sides
### IP address management
- Layer 3 interfaces
- VLAN interfaces
- Management interfaces
- IP address, subnet mask/CIDR block, default gateway, DNS (optional)
![[Pasted image 20240513124200.png]]
# VLANs
### VLAN assignment
- each device port should be assigned a VLAN
### Trunking
- connecting switches together
- multiple VLANs in a single link
### Tagged and Untagged VLANs
- a non-tagged frame is on the default VLAN
	- also called the native VLAN
- trunks ports will tag the outgoing frames
	- and remove the tag on incoming frames
![[Pasted image 20240513124332.png]]
# LAG and mirroring
### Port bonding / Link aggregation (LAG)
- multip0le interfaces acts like one big interface
- LACP (Link Aggregation Control Protocol)
	- adds additional automation and management
### Port mirroring
- copy traffice from one interface
- used for packet captures ,IDS
- mirror traffic on the same switch
- mirror traffic from one switch to another
![[Pasted image 20240513124547.png]]
# Port mirroring
### Examine a copy of the traffic
- port mirror (SPAN) , network tap
![[Pasted image 20240513124605.png]]
# Jumbo frames
### Ethernet frames with more than 1,500 bytes of payload
- up to 9,216 bytes (9,000 is the accepted norm)
### Increase transfer efficiency
- per-packet size
- fewer packets to /switch/routes
### Ethernet devices must support jumbo frames
- switches, interface cards
- not all devices are compatible with other
![[Pasted image 20240513125233.png]]
# Ethernet flow control
### Is non-deterministic
- you never know just how fast or slow traffic will flow
### If busy, tell other devices to slow down
- switches only have so much buffer
### One popular flow control method is IEE 802.3x
- the "pause" frame
### Enhancements have been made over the years
- incorporates CoS (Class of Service)
![[Pasted image 20240513125410.png]]
![[Pasted image 20240513125427.png]]
# Port security
### Prevent unauthorized users from connecting to a switch interface
- alert or disable the port
### Based on the source MAC address
- even if forwarded from elsewhere
### Each port has its own config
- unique rules for every interface
# Port security operation
### Configure a maximum number of source MAC addresses on an interface
- you decide how many is too many
- you can also configure specific MAC addresses
### The switch monitors the number of unique MAC addresses
- maintains a list of every source MAC addresses
### Once you exceed the maximum, port security activates
- default is to disable the interface
