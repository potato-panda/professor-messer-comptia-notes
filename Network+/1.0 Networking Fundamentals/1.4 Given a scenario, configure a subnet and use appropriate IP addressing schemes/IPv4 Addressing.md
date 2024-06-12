# Networking with IPv4
### IP address, e.g., 192.168.1.165
- every device needs a unique IP address
### Subnet mask, e.g., 255.255.255.0
- used by the local device to determine what subnet it's on
	- isn't (usually) transmitted across the network
	- you'll ask for this all the time: **What's the subnet mask of this network?**
		- important routing outside the IP subnet, and send info to a default gateway
		- if the device doesn't know it's own subnet then it doesn't know what information should be communicated locally and what information should be sent to the default gateway
		- therefore, make sure the subnet mask is configured
### Default gateways e.g. 192.168.1.1
> is the IP address that's on the same local subnet as your IP address
- router that allows you to communicate outside your local subnet
- default gateway must be an IP address on the local subnet
> will commonly configure additional setting no listed above: That's the domain name system server, or DNS server

# Special IPv4 addresses
### Loopback address
- address to yourself
- ranges from 127.0.0.1 to 127.255.255.254
- easy way to self-reference (ping 127.0.0.1)
> you would know the IP stack of the machine is working properly if you get a response pinging 127.0.0.1
### Reserved addresses
- reserved for future use or testing
- 240.0.0.1 to 254.255.255.254
- all "Class E" addresses
### Virtual IP addresses (VIP)
- Not associated with a physical network adapter
- Virtual machine, internal router address

# IPv4 addresses
### Internet Protocol version 4
- OSI Layer 3 address
![[Pasted image 20240504173252.png]]

# Dynamic Host Configuration Protocol (DHCP)
### IPv4 address configuration used to be a manual process
- IP address, subnet mask, gateway, DNS servers, NTP servers, etc
### Dynamic Host Configuration Protocol
- provides automatic address and IP configuration for almost all devices

# Automatic Private IP Addressing (APIPA)
### A link-local address
> DHCP may not be available
- can only communicate to other local devices
- no forwarding by routers
### IETF has reserved 169.254.0.1 to 169.254.255.254
> is how you can know if you can assign one
- first and last 256 addresses are reserved
- functional block of 169.254.1.0 to 169.254.254.255
### Automatically assigned
- uses ARP to confirm the address isn't currently in use
