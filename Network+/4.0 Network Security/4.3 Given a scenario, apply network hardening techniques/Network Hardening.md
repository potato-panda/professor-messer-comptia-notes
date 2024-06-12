# Secure SNMP
### Secure Simple Network Management Protocol
- monitor and control servers, switches, routers, firewalls, and other devices
### Different versions through the years
- SNMPv1 and SNMPv3 do not encrypt network traffic
### SNMPv3
- version 3 added encrypted communication
- not all devices support it
- use it everywhere you can
# Router Advertisement (RA) guard
### IPv6 includes periodic router announcements
- automatic configuration for network devices
### A rogue device could pretend to be a router
- could be part of an on-path attack, denial of service, etc
### Switches can validate the RA messages
- admins define policies to check the RA messages
![[Pasted image 20240514182322.png]]
# Port security
### Prevent unauthorized users form connecting to a switch interface
- alert or disable the port
### Based on the source MAC address
- even if forwarded from elsewhere
### Each port has it's own config
- unique rules for every interface
# Port security operation
### Configure a maximum number of source MAC addresses on an interface
- you decide how many is too many
- you can also configure specific MAC addresses
### The switch monitors the number of unique MAC addresses
- maintains a list of every source MAC address
### Once you exceed the maximum, port security activates
- default is to disable the interface
# Dynamic ARTP inspection (DAI)
### ARP is powerful
- but has no built-in security
### Prevent those nasty on-path attacks
- stops ARP poisoning at the switch level
### Relies on AHCP snooping for intel
- knowing every devices' IP can be valuable information
### Intercept all ARP requests and responses
- invalid IP-to-MAC address bindings are dropped
- only valid requests make it through
# Control plane policing
### Control plane manages the device
- data plane performs the operational processes
### Protect against DoS or reconnaissance
- defines a QoS filter to protect the control plane
- control packets should have the priority
### Manage traffic
- prioritize management traffic
- block unnecessary control plane traffic types (i.e. non-SSH)
- rate limit the control plane traffic flows
# Private VLANs
### Port isolation
- restrict access between interfaces
- even when they're in the same VLAN
### You might already be using private VLANs
- your home internet can't direct connect to another home
- hotel room access is limited to Internet connectivity
# Disabling unused interfaces
### Enabled physical ports
- conference rooms
- break rooms
### Administratively disable unused ports
- more to maintain, but more secure
### Network access control (NAC)
- 802.1X controls
- you can't communication unless you are authenticated
# Disable unnecessary ports and services
### Every open port is a possible entry point
- close everything except required ports
### Control access with a firewall
- NGFW would be ideal
### Unused or unknown services
- installed with the OS or form other applications
### Applications with broad port ranges
- open port 0 through 65,535
### Use Nmap or similar port scanner to verify
- ongoing monitoring is important
# Changing default credentials
### Most devices have default usernames and passwords
- change yours!
### The right credentials provide full control
- admin access
### Very easy to find the defaults for your AP or router
- https://www.routerpasswords.com
# Password complexity and length
### Make your password strong
- resist guessing or brute-force attack
### Increase password entropy
- no single words, no obvious passwords
	- what's the name of you dog?
- mix upper and lower case and use special characters
	- don't replace a o with 0, and t with 7
### Stronger passwords are at least 8 characters
- consider a phrase or set of words
# DHCP snooping
### IP tracking on a layer 2 device (switch)
- the switch is a DHCP firewall
- trusted: routers, switches, DHCP servers
- untrusted: other computers, unofficial DHCP servers
### Switch watches for DHCP conversations
- adds a list of untrusted devices to a table
### Filters invalid IP and DHCP information
- static IP addresses
- devices acting as DHCP servers
- other invalid traffic patterns
# Change default VLAN
### All access ports (non-trunk ports) are assigned to a VLAN
- without any additional security (802.1X), anyone connecting will be part of the default VLAN
### The default VLAN might also be used by default for control plane access/management
- don't put users on the management VLAN
- change the management VLAN to something exclusive
### Assign unused interfaces to a specific non-routable, non-forwarding VLAN
- a "dead-end" or "impasse" VLAN
![[Pasted image 20240514184823.png]]
# Upgrading firmware
### Many network devices do not use a traditional operating system
- all updates are made to firmware
### The potential exists for security vulnerabilities
- upgrade the firmware to a non-vulnerable version
### Plan for the unexpected
- always have a rollback plan
- save those firmware binaries
# Patch management
### Incredibly important
- system stability
- security fixes
### Service packs
- all at once
### Monthly updates
- incremental  and important)
### Emergency out-of-band updates
- zero-day and important security discoveries
![[Pasted image 20240514185343.png]]
# Role-based access
### Not everyone connecting to a switch or router needs the same level of access
- admins, help desk, management, API access
### Many devices allow the configuration of specific roles
- rights and permissions are based on the role
- admins can configure and reboot the device
- help desk can view statistics
- API access can't interactive login/SSH
# Access Control lists (ACLs)
### Allow or disallow traffic based on tuples
- groups of categories
- source IP, destination IPs, port number, time of day, application, etc
### Restrict access to network devices
- limit by IP addresses or other identifier
- prevent regular user / non-admin access
### Be careful when configuring these
- you can accidentally lock yourself out
# Firewall rules
### Manage access from the firewall
- additional security options
- username, VPN, MFA
### Most firewall rules include an implicit deny
- if there's no explicit rule, then traffic is blocked
- these implicit deny rules aren't usually logged
### Some firewall admins will add explicit deny rules
- anything denied by a rule is logged by default
- can be useful for identifying reconnaissance or access attempts
![[Pasted image 20240514185832.png]]
