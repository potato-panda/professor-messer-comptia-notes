# [[Advanced Networking Devices#Network-based firewalls|Network-based firewalls]]
# [[Firewall Types#Network-based Firewalls|Network-based firewalls]]
# Ports and protocols
### Make forwarding decisions based on protocol (TCP/UDP) and port number
- trad port-based fw
- add to an NGFW for additional security policy options
### Based on destination protocol and port
- web server: tcp/80, tcp/443
- SSH server: tcp/22
- Microsoft RDP: tcp/3389
- DNS query: udp/53
- NTP: udp/123
# Firewall rules
### A logical path
- usually top-to-bottom
### Can be very general or very specific
- specific rules are usually at the top
### Implicit deny
- most fw include a deny at the bottom
	- even if you didn't add one
### [[Network Hardening#Access Control lists (ACLs)|ACL]]
# [[Defence in Depth#Screened subnet|Screen subnet]]
### An additional layer of security between you and Internet
- public access to public resources
- private data remains inaccessible
# IPS rules
- usually integrated into an NGFW
### Different ways to find malicious traffic
- looks at traffic as it passes
### Signature-based
- look for perfect match
### Anomaly-based
- build a baseline of what's "normal"
- usual traffic patterns are flagged
### You determine what happens when unwanted traffic appears
- block, allow, send an alert, etc
### Thousands of rules
### Rules can be customized by group
- or individual rules
### This can take time to find the right balance
- security / alert "noise" / false positives