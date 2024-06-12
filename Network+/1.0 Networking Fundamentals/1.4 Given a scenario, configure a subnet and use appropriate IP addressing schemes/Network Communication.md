# Unicast
### One machine sending information to another machine
- one-to-one
### Send information between two systems
### Web surfing, file transfer
### Does not scale optimally for real-time streaming media
### Commonly with IPv4 and IPv6

# Broadband
### Send information to everyone at once
- one-to-all
### One packet, received by everyone
### Limited scope (usually to local IP subnet)
- only the broadcast domain
### Routing updates, ARP updates
- lots of routing protocols they rely on broadcast to send updates to machines on the network
	- On IPv4, ARP request use broadcast extensively
### Used in IPv4
- too many broadcasts on the network can create performance problems for all other machines
- used extensively
### Not used in IPv6
- uses multicast instead, does not support broadcast
> corrected the IPv4 performance issue in IPv6 by limiting the scope of what's sent to all of the devices, so you see multicast used in IPv6 instead of broadcast

# Multicast
### Delivery of information to **interested** systems
- one-to-many-of-many
### Multimedia delivery, stock exchanges, dynamic routing updates
### Very specialized 
- difficult to scale across large networks
### Used in both IPv4 and IPv6
- extensively used in IPv6

# Anycast
### Single destination IP address has multiple paths to two or more endpoints
- one-to-one-of-many
- Used in both v4 and v6
### Configure the same anycast address on different devices
- they look like any other unicast address
### Packets sent to an anycast address are delivered to the closest interface
- announce the same route out of the mult0ple data centers, clients use the data center closest to them
- Anycast DNS
> Commonly used with DNS servers