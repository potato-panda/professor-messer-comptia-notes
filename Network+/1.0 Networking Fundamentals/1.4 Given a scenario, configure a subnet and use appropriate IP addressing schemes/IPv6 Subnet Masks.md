# Assigning IPv6 addresses
### Internet Assigned Numbers Authority (IANA) provides address blocks to RIRs (Regional Internet Registries)

### RIRs assigns smaller subnet blocks to ISPs (Internet Service Providers)
### ISP assigns a /48 subnet to the customer

![[Pasted image 20240506224827.png]]

# Subnetting the IPv6 address
### 2600:DDDD:1111
![[Pasted image 20240506224941.png]]

### 16 subnet bits = 65,536 total subnets
### 2^64 hosts
- that's about 18 million trillion hosts per subnet
### the Prefix and host ID are both 64 bits long
### Subnet address:
![[Pasted image 20240506225110.png]]
![[Pasted image 20240506225147.png]]

# Tunneling IPv6
### 6to4 addressing
- send IPv6 over than existing IPv4 network
- creates an IPv6 address based on the IPv4 address
- requires specific relay router
- no support for NAT
### 4in6 tunneling
- tunnel IPv4 traffic on an IPv6 network
# Teredo / Miredo
### Tunnel IPv6 through NATed IPv4
- allows e2e IPv6 through an IPv4 network
- no special IPv6 router required
- temporary use communication
	- until will we have IPv6 native networks soon?
### Miredo
- open-source Teredo for Linus, BSD Unix, and Max OS X
- full functionality
# Dual-stack routing
### Dual-stack IPv4 and IPv6
- run both at the same time
- interfaces will be assigned multiple address types
### IPv4
- configured with IPv4 addresses
- maintains an IPv4 routing table
- uses IPv4 dynamic routing protocols
### IPv6
- configured with IPv6 addresses
- maintains a separate IPv6 routing table
- uses IPv6 dynamic routing protocols
# Howdy, neighbour
### There's no ARP in IPv6
- so how do you find the MAC address of a device?
### Neighbor Solicitation (NS)
- sent as a multicast
### Neighbor Advertisement (NA)
![[Pasted image 20240506232639.png]]
# Neighbor Discovery Protocol
### No broadcasts
- operates using multicast with ICMPv6
### Neighbor MAC Discovery
- replaces the IIPVv4 ARP
### SLAAC (Stateless Address Autoconfiguration)
- automatically configure an IP address without a DHCP server
### DAD (Duplicate Address Detection)
- no duplicate IPs
### Discover routers
- router solicitation and router advertisement
# Finding Router
### Use the Neighbor Discovery Protocol
![[Pasted image 20240506232934.png]]
### Router also send unsolicited RA messages
- from the multicast destination of ff02::1
### Transfers IPv6 address information, prefix value, and prefix length, etc.
