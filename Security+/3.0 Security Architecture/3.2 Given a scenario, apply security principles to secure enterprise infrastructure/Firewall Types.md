# The universal security control
### Standard issue
- home, office, and in OS
### Control the flow of network traffic
- everything passes through the firewall
### Corporate control of outbound and inbound data
- sensitive materials
### Control of inappropriate content
- NSFW, parental controls
### Protection against evil
- AV, anti-malware
# Network-based firewalls
### Filter traffic by port number or app
- OSI layer 4 vs OSI layer 7
- traditional vs NGFW
### Encrypt traffic
- VPN between sites
### Most firewalls can be layer 3 devices (routers)
- often sits on the ingress/egress of network
- NAT functionality
- authenticate dynamic routing communication
# UTM / All-in-one security appliance
- Unified Threat Management (UTM) / Web security gateway
- URL / content inspection
- malware inspection
- spam filter
- CSU/DSU
- router/switch
- firewall
- IDS/IPS
- bandwidth shaper
- VPN endpoint
### Only layer 4
# Next-generation firewall (NGFW)
### OSI app layer (7)
- all data in every packet
### Different names
- app layer gateway
- stateful multilayer inspection
- deep packet inspection
### Requires some advanced decodes
- every packet must be analyzed and categorized before security decision is determined
### Network-based Firewalls
- control traffic flows based on the app
	- Microsoft SQL Server, Twitter, YouTube
### IPS
- ID the app
- application app-specific vuln signatures to the traffic
### Content filtering
- URL filters
- control website traffic by category
# Web application firewall (WAF)
### Not like a "normal" firewall
- applies rules to HTTP/HTTPS conversations
### Allow/deny based on expect input
-unexpected input is a common method of exploiting an app
### SQL injection
- add your own commands to app's SQL query
### Major focus of Payment Card Industry Data Security Standards (PCI DSS)
![[Pasted image 20240607142231.png]]