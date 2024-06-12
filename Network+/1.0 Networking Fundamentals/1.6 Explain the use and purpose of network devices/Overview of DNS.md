# Domain Name System
### Translates human-readable names into computer-readable IP addresses
- you only need to remember www.google.com
# Hierarchical
### Follow the path
# Distributed database
- many DNS servers
- 13 root server clusters (1000 actual servers)
- hundreds of generic top-level domains (gTLD) - .com, .org, .net, etc...
- over 275 country code TLDs (ccTLD) - .us, .ca, .uk
# The DNS Hierarchy
![[Pasted image 20240509134507.png]]
# FQDN (Fully Qualified Domain Name)
![[Pasted image 20240509134608.png]]
# Internal vs External DNS
### Internal
- managed on internal servers
- configured and maintained by the local team
- contains DNS information about internal devices
- DNS server on Windows Server
### External
- Often managed by a third-party
- does not have internal device information
- Google DNS, Quad9
# Recursive and iterative DNS queries
### Many ways to get what you need
### Recursive query
- delegate the lookup to a DNS  server
- the server does the work and reports back
- large DNS cache provides a speed advantage
### Iterative query
- do all queries yourself
- DNS cache is specific to you
# Recursive DNS query
![[Pasted image 20240509135021.png]]
# Iterative DNS query
![[Pasted image 20240509135051.png]]
# The authority
### Authoritative
- DNS server is the authority for the zone
### Non-authoritative
- does not contain the zone source files
- probably cached information
### TTL (time to live)
- configured on the authoritative server
- specifies how long cache is valid
- a very long TTL can cause problems if changes are made
![[Pasted image 20240509135223.png]]
![[Pasted image 20240509135243.png]]
# Lookups
### Forward looup
- provide DNS server with an FQDN
- DNS server provides an IP address
### Reverse DNS
- provide DNS server with an IP address
- DNS server provided an FQDN
### Forward lookup
![[Pasted image 20240509135445.png]]
### Reverse lookup
![[Pasted image 20240509135502.png]]