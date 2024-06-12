# Layer 3 capable switch
### A switch (L2) and router (L3) in the same physical device
- L3 switch
- L2 router?
### Switching still operates at Layer 2, routing still operates at L3
- there's nothing new or special here
# Wireless networks everywhere
### Wireless networking is pervaise
- and you probably don't just have one access point
### Your AP may not even be in the same building
- one or more at every remote site
### Configurations may change at any moment
- Access policy, security policies, AP configs
### The network should be invisible to your users
- seamless network access, regardless of role
# Wireless LAN controllers
### Centralized management of APs
- a single "pane of glass"
### Deploy new APs
### Performance and security monitoring
### Configure and deploy changes to all sites
### Report on AP use
### Usually a proprietary system
- wireless controller is usually paired with the APs
# Balancing the load
### Distribute the load
- multiple servers
- invisible to the end-user
### Large-scale implementations
- web server farms, database farms
### Fault tolerance
- server outages have no effect
- very fast convergence
# Load balancer
### Configurable load
- manage across servers
### TCP offload
- takes server's protocol overhead
### SSL offload
- takes server's encryption/decryption overhead
### Caching
- fast response
### Prioritization
- QoS
### Content switching
- application-centric balancing
![[Pasted image 20240510154923.png]]
# IDS and IPS
###  Intrusion Detection System/ Intrusion Prevention System
- watch network traffic
### Intrusions
- exploits against operating systems, applications, etc
- Buffer overflows, cross-site scripting, other vulnerabilities
### Detection vs Prevention
- detection: alarm or alert
# Proxies
### Sits between the users and the external network
### Receives the user requests and sends the request on their behalf (the proxy)
### Useful for caching information, access control, URL filtering, content scanning
### Applications may need to know how to use the proxy (explicit)
### Some proxies are invisible (transparent)
![[Pasted image 20240510155227.png]]
# Application Proxies
### Most proxies in use are application proxies
- proxy understand the way the application works
### A proxy may only know one application
- HTTP
### Many proxies are multipurpose proxies
- HTTP, HTTPS, FTP, etc
# VPN concentrator
### VPN
- encrypted (private) data traversing a public network
### Concentrator / head-end
- encryption/decryption access device
- often integrated into a firewall
### Many deployment options
- specialized cryptographic hardware
- software-based options available
### Used with client software
- sometimes build into the OS
# VoIP technologies
### PBX (Private Branch Exchange)
- the "phone switch"
- connects to phone provider network
- analog telephone lines to each desk
### VoIP PBX
- integrate VoIP devices with a corporate phone switch
### Voice gateway
- convert between VoIP protocols and traditional PSTN protocols
- often built-in to the VoIP PBX
# Network-based firewalls
### Filter traffic by port number or application
- traditional vs. NGFW (Next generation firewalls)
### Encrypt traffic
- VPN between sites
### Most firewalls can be layer 3 devices (routers)
- often sites on the ingress/egress of the network
- Network Address Translation (NAT)
- Dynamic routing