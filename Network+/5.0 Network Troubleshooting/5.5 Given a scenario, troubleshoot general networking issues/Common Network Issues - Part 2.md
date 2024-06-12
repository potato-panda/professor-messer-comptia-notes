# Rogue DHCP server
### IP addresses assigned by a non-authorized server
- there's no inherent security in DHCP
### Client is assigned an invalid or duplicate address
- intermittent connectivity, no connectivity
### Disable rogue DHCP communication
- enable DHCP snooping on your switch
- Authorized DHCP servers in Active Directory
### Disable the rogue
- renew the IP leases
# Exhausted DHCP scope
### Client received an APIPA address
- local subnet communication only
### Check the DHCP server
- add more IP addresses if possible
### IP address management (IPAM) may help
- monitor and report on IP address shortages
### Lower the lease time
- especially if there are a lot of transient users
# IP configuration issues
### Communication to local IP addresses
- but no outside subnets
### No IP communication
- local or remote
### Communicate to some IP addresses
- but not others
# Troubleshooting IP configurations
### Check your documentation
- IP address, subnet mask, gateway, DNS
### Monitor the traffic
- examine local broadcasts
- difficult to determine subnet mask
### Check devices around you
- confirm your subnet mask and gateway
### Traceroute and ping
- the issue might be your infrastructure
- ping local IP, default gateway, and outside address
# Low optical link budget
### Fiber networks rely on the transmission of light
- block the light, block the network
### Attenuation
- a challenge over long distances
- or with dirty connectors
### Always check with a light meter
- equipment documentation will specify the required amount light
# Certificate issues
### Security alerts and invalid certificates
- something isn't quite right
- should raise your interest
### Look at the certificate details
- click the lock icon
- may be expired or the wrong domain name
- the certificate may not be properly signed (untrusted certificate authority)
- correct time and date is important
# Hardware failure
### No response
- application doesn't respond
### Confirm connectivity
- without a ping, you're not going to connect
### Run a traceroute
- see if you're being filtered
- should make it to the other side
### Check the server
- lights? fire?
# Incorrect firewall settings
### Applications not working
- based on the application in use or the protocol and port
### Check the host-based firewall settings
- accessibility may be limited to an admin
- managed from a central console
### Confirm the network-based firewall config
- check the policy list and logs
### Take a packet capture
- the traffic may never make it to the network
- dropped by the OS
# Incorrect VLAN configurations
### Check VLAN assignments on the switch
- this is one of the most common issues you'll find
### Confirm the data and voice VLAN assignments
- useful when using VOIP phones
### Validate the physical interface with the VLAN number
- also important for trunks
# DNS issues
### Web browsing doesn't work
- the internet is broken!
### Ping works, browser doesn't
- there isn't a communication problem
### Application aren't communicating
- they often use names and not IP addresses
# Troubleshooting DNS issues
### Check your IP configuration
- is the DNS IP address correct?
### Use nslookup or dig to test
- does resolution work?
### Try a different DNS server
- Google at 8.8.8.8
- QuadNine at 9.9.9.9
# NTP issues (Network Time Protocol)
### Some cryptography is very time sensitive
- Active Directory requires clocks set within five minutes of each other
### Kerberos communication uses a time stamp
- if the ticket shown during authentication is too old, it's invalid
### Client can't login
- check the timestamp of the client and the server
### Configure NTP on all devices
- Automate the clock setting
# BYOD
### Bring your own technology
### Employee owns the device
- need to meet company requirements
### Difficult to secure
- it's both a home device and a work device
- how is data protected?
- what happens to the data when a device is sold or traded in?
### Use an MDM (Mobile Device Manager)
# Licensed feature issues
### Features are often individually licensed
- requires payment or some type of license agreement
### Some features may not be available
- a license key unlocks functionality
### This can cause problems during an upgrade or configuration update
- test your changes in the lab
![[Pasted image 20240516172654.png]]
# Network performance issues
### There's never just one performance metric
- series of technologies working together
### I/O bus, CPU speed, storage access speed, network throughput, etc
- one of these can slow all of the others down
### You must monitor all of them to find the slowest one
- this may be more difficult than you might expect
![[Pasted image 20240516172835.png]]
# Resolving the network bottleneck
![[Pasted image 20240516172825.png]]