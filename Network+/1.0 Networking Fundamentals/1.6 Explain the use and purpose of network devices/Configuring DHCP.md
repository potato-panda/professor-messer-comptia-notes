# Scope properties
### IP address range
- and excluded addresses
### Subnet maks
### Lease duration
### Other scope options
- DNS server
- Default gateway
- VOIP servers
# DHCP pools
### Grouping of IP addresses
- each subnet has its own scope
- 192.168.1.0/24
- 192.168.2.0/24
- ...
### A scope is generally a single contiguous pool of IP addresses
- DHCP exceptions can be made inside of the scope
# DHCP address assignment
### Dynamic assignment
- DHCP server has a big pool of addresses to give out
- Addresses are reclaimed after a lease period
### Automatic assignment
- Similar to dynamic allocation
- DHCP servers keep a list of past IP assignments
- You'll always get the same IP address
# DHCP address allocation
### Static assignment
- administratively configured
### Table of MAC addresses
- each MAC address has a matching IP address
### Other names
- static DHCP assignment
- Static DHCP 
- address reservation
- IP reservation
# Address reservation
# DHCP leases
### Leasing your address
- only temporary
- but can be seem permanent
### Allocation
- assigned a lease time by the DHCP server
- administratively configured
### Reallocation
- reboot computer
- confirms the lease
### Workstation can also manually release the IP address
- moving to another subnet
# DHCP renewal
### T1 timer
- check in with the lending DHCP server to renew the IP address
- 50% of the lease time (by default)
### T2 timer
- if original DHCP server is down, tries rebinding with any DHCP server
- 87.5% of the lease time (7/8ths)
# The DHCP lease process
![[Pasted image 20240509133751.png]]