# [[Advanced Networking Devices#VPN|VPNs]]
# Client-to-site VPN
### On-demand access from remote device
- software connects to a VPN concentrator
### Some software can be configured as always-on
![[Pasted image 20240515124016.png]]
![[Pasted image 20240515124310.png]]
> Data sent from laptop to VPN over internet is encrypted and decrypted by the VPN concentrator and on the reverse from the network, data sent is encrypted on the VPN concentrator and decrypted on the laptop
# Site-to-site VPN
### Always-on
- or almost always
### Firewall often acts as VPN concentrators
- probably already have firewalls in place
![[Pasted image 20240515124252.png]]
# Clientless VPNs
### Hypertext Markup Language version 5
- language commonly used in web browsers
### Included comprehensive API support
- APIs
- Web Cryptography API
### Create a VPN tunnel without a separate VPN application
- nothing to install
### Use an HTML5 compliant browser
- communicates directly to the VPN concentrator
# Full Tunnel
![[Pasted image 20240515124505.png]]
> All connections to outside networks (www.professormesser.com) go through VPN concentrator before routed to them
# Split Tunnel
![[Pasted image 20240515124646.png]]
> Admins can determine which connections go through the VPN tunnel and what doesn't
# Remote desktop connection
### Share a desktop from a remote location
- it's like you're right there
### RDP (Microsoft Remote Desktop Protocol)
- clients for MacOS, Linux, and others as well
### VNC (Virtual Network Computing)
- Remote Frame Buffer (RFB) protocol
- clients for many operating systems
- many are open source
### Commonly used for technical support
- and for scammers
# Remote desktop gateway
### Combine a VPN with Microsoft Remote Desktop
- securely access RDP servers from the outside
### Client connects to the Remote Desktop Gateway
- secure SSL tunnel
- many authentication options
### Remote Desktop Gateway connects internally to RDP servers over tcp/3389
- no special configurations required
- Gateway is the proxy between the SSL tunnel and the Remote Desktop protocol
![[Pasted image 20240515125343.png]]
> Flows left to right
# SSH (Secure Shell)
### Encrypted console communication - tcp/22
### Looks and acts the same as Telnet - tcp/23
# Cloud-hosted virtual desktops
### A virtual desktop infrastructure (VDI) in the cloud
- users connect to a pre-built desktop
### Access from almost any OS
- Windows, MacOS, Linux, iOS, Chromebook, web browser
### Virtual NIC
- All communication in the desktop are local to the virtual desktop
- no sensitive information sent from the local device
# Authentication and authorization
### 2008 until May 2011 - Subway Sandwiches
- 200 locations were breached
- point of sales systems were equipped with remote desktop software
- 80,000 credit cards, millions of dollars of unauthorized purchases
### Significant security issues
- default credentials and brute force attacks
- remote access requires More security, not less
### Once connected, authorization is key
- access rights should be limited
# Out-of-band management
### The network isn't available
- or the device isn't accessible from the network
### Most devices have a separate management interface
- usually a serial connection / USB
### Connect a modem
- dial-in to manage the device
### Console router / comm server
- out-of-band access for multiple devices
- connect to the console router, then choose where you want to go