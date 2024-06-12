# Jump server
### Access secure network zones
- provides an access mechanism to a protected network
### Highly-secured device
- hardened and monitored
### SSH / Tunnel / VPN to the jump server
- RDP, SSH, or jump from there
![[Pasted image 20240607134633.png]]
### A significant security concern
- compromise of the jump server is a significant breach
# Proxies
### Sits between the users and the external network
### Receives the user requests and send the request on their behalf (the proxy)
### Useful for caching information, access control, URL filtering, content scanning
### Apps may need to know how to use the proxy (explicit)
### Some proxies are invisible (transparent)
![[Pasted image 20240607134754.png]]
# Application proxies
### One of the simplest "proxies" is NAT
- network-level proxy
### Most proxies in use are app proxies
- proxy understands the way the app works
### Proxy may only know one app
- HTTP
### Many proxies are multipurpose proxies
- HTTPS, HTTPS, FTP, etc
# Forward proxy
### An "internal" proxy
- commonly used to protect and control user access to the internet
![[Pasted image 20240607135056.png]]
# Reverse proxy
### Inbound traffic from the Internet to your internal service
![[Pasted image 20240607135119.png]]
# Open proxy
### A third-party, uncontrolled proxy
- can be significant security concern
- often used to circumvent existing security controls
![[Pasted image 20240607135222.png]]
# Balancing the load
### Distribute the load
- multiple servers
- invisible to the end-users
### Large-scale impl
- web server farms, db farms
### Fault tolerance
- server outages have no effect
- very fast convergence
# Active/active load balancing
### Configurable load
- manage across servers
### TCP offload
- protocol overload
### SSL offload
- encryption/decryption
### Caching
- fast response
### Prioritization
- QoS
### Content switching
- app-centric balancing
![[Pasted image 20240607135517.png]]
# Active/passive load balancing
### Some servers are active
- others are on standby
### If an active server fails, the passive servers takes its place
# Sensors and collectors
### Aggregate information from network devices
- built-in sensors, separate devices
- integrated into switches, routers, servers, firewalls, etc
### Sensors
- IPS, firewall logs, auth logs, web server access logs, db transaction logs, email logs
### Collectors
- proprietary consoles (IPS, firewall), SIEM consoles, syslog servers
- many SIEMs include a correlation engine to compare diverse sensor data