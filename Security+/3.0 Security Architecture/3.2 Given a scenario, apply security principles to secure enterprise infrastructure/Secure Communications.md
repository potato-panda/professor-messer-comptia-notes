# [[Remote Access#VPNs|VPNs]]
# Encrypted tunnel
### Keep data private across the public Internet
- encryption is the key
### Encrypt your data
- add new headers and trailers
### Decrypt on the other side
- original data is delivered
![[Pasted image 20240607151234.png]]
# SSL/TLS VPN (Secure Sockets Layer VPN)
### Uses common SSL/TLS protocol (tcp/443)
- (almost) no firewall issues
### No big VPN clients
- usually remote access comms
### Authn users
- no requirement for digital certs or shared passwords (like IPsec)
### Can be run from browser or from (usually light) VPN client
- across many OS
### On-demand access from a remote device
- software connects to a VPN concentrator
[[Remote Access#Client-to-site VPN]]
### Some software can be configured as always-on
# [[Remote Access#Site-to-site VPN|Site-to-site IPsec VPN]]
# [[Network Types#Software Defined Networking in a Wide Area Network (SD-WAN)|SD-WAN]]
# Secure Access Service Edge (SASE)
### Update secure access for cloud services
- securely connect from different locations
### Secure Access Service Edge
- "next generation" VPN
### Security tech are in the cloud
- located close to existing cloud services
### SASE clients on all devices
- streamlined and automatic
![[Pasted image 20240607152121.png]]
# Selection of effective controls
### Many different security options
- selecting the right choice can be challenging
### VPN
- SSL/TLS VPN for user access
- IPsec tunnels for site-to-site access
### SD-WAN
- manage network connectivity to the cloud
- does not adequately address security concerns
