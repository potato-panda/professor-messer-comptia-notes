# Device placement
### Every network is different
- often similarities
### Firewalls
- separate trusted from untrusted
- provide additional security checks
### Other service may require their own security tech
- honeypots, jump server, load balancers, sensors
# Security zones
### Zone-based security techs
- more flexible (and secure) then IP address ranges
### Each area of the network is associated with a zone
- trusted, untrusted
- internal, external
- inside, Internet, servers, dbs, screened
### This simplifies security policies
- trusted to untrusted
- untrusted to screened
- untrusted to trusted
### Example
![[Pasted image 20240607133308.png]]
![[Pasted image 20240607133314.png]]
# Attack surface
### How many ways into your home?
- doors, windows, basements
### Everything can be a vulnerability
- app code
- open ports
- auth process
- human error
### Minimize the surface
- audit the code
- block ports on the firewall
- monitor network traffic in real-time
# Connectivity
### Everything contributes to security
- including the network connection
### Secure network cabling
- protect the physical drops
### App-level encryption
- hard work is already done
### Network-level encryption
- IPsec tunnels, VPN connections