# DHCP
### IPv4 address configuration used to be manual
- IP address, subnet mask, gateway, DNS servers, NTP servers, etc
### October 1993 - the bootstrap protocol
- BOOTP
### BOOTP didn't automatically define everything
-  some manual configurations were still required
- BOOTP also didn't know when a IP address might be available again
### Dynamic Host Configuration Protocol
- initially released in 1997, updated through the years
- provided automatic address / IP configuration for almost all devices
# Step 1: Discover
![[Pasted image 20240508164919.png]]
# Step 2: Offer
![[Pasted image 20240509130022.png]]
# Step 3: Request
![[Pasted image 20240509130146.png]]
# Step 4: Acknowledgement
![[Pasted image 20240509130641.png]]
# Managing DHCP in the enterprise
### Limited communication range
- uses the IPv4 broadcast domain
- stops at a router
### Multiple servers needed for redundancy
- across different locations
### Scalability is always an issue
- may not want/need to manage DHCP servers at every remote location
### You're going to need a little help(er)
- send DHCP request across broadcast domains
# DHCP relay
![[Pasted image 20240509131417.png]]
# Offer with DHCP relay
![[Pasted image 20240509131520.png]]
![[Pasted image 20240509131600.png]]