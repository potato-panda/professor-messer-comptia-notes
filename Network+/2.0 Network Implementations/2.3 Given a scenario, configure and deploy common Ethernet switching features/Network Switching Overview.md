# The switch
### Forward or drop frames
- based on the destination MAC address
### Gather a constantly updating list of MAC addresses
- builds the list based on the source MAC address of incoming traffic
### Maintain a loop-free environment
- using Spanning Tree Protocol (STP)
# Frame switching
![[Pasted image 20240510180601.png]]
![[Pasted image 20240510180630.png]]
![[Pasted image 20240510180636.png]]
![[Pasted image 20240510180646.png]]
# Frame switching between switches
![[Pasted image 20240510180700.png]]
![[Pasted image 20240510180724.png]]
![[Pasted image 20240510180733.png]]
![[Pasted image 20240510180744.png]]
 ![[Pasted image 20240510180802.png]]
# Learning the MACs
### Switches examine the incoming traffic
- makes a note of the **source** MAC address
### Adds unknown MAC addresses to the MAC address table
- sets the output interface to the received interface
![[Pasted image 20240510180908.png]]
![[Pasted image 20240510180923.png]]
![[Pasted image 20240510180932.png]]
![[Pasted image 20240510180952.png]]
# Flooding for unknown MACs
### The switch doesn't always have a MAC address in the table
### When in doubt, send the frame to all devices
![[Pasted image 20240510181040.png]]
![[Pasted image 20240510181046.png]]
![[Pasted image 20240510181118.png]]
# Address Resolution Protocol
### Determine a MAC address based on an IP address
- you need the hardware address to communication
### arp -a
- view local ARP table
# NDP (Neighbor Discovery Protocol)
### No broadcasts!
- operates using multicast with ICMPv6
### Neighbor MAC Discovery
- replaces the IPv4 ARP
### SLAAC (Stateless Address Autoconfiguration)
- automatically configure an IP address without a DHCP server
### DAD (Duplicate Address Detection)
- no duplicate IPs!
# Howdy, Neighbor
### There's no ARP in IPv6
- so how do you have find the MAC address of a device?
### Neighbor Solicitation (NS)
- sent as a multicast
### Neighbor Advertisement (NA)
![[Pasted image 20240510182145.png]]
> Slightly different than NDP, but process is similar
# Power over Ethernet (PoE)
### Power provided on an Ethernet cable
- one wire for both network and electricity
- phones, cameras, wireless access points
- useful in difficult-to-power areas
### Power provided at the switch
- built-in power (coming from the switch) - Endspans
- In-line power injector (from injector) - Midspans
### Power modes
- Mode A: Power on the data pairs (Gigabit is using all the wires, so send power and data on the same wires)
- Mode B: Power on the spare pairs (unused wires on 10/100 Mb/s Ethernet)
# PoE and POE+
### PoE: IEEE 802.3af-2003
- original PoE specification
- now part of the 802.3 standard
- 15.4 watts of DC power
- maximum current of 350 mA
### POE+: IEEE 802.3at-2009
- updated specfication
- now part of the 802.3 standard
- 25.5 watts of DC power
- max current 600 mA