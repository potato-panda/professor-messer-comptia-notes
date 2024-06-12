# Threat Vector
### Method used by the attacker
- gain access or infect the target
- also called "Attack Vectors"
### A lot of work goes into finding vulnerabilities in these vectors
- some are more vulnerable than others
### IT Security Professionals spend their career watching these vectors
- protect existing vectors
- find new vectors
# Message-based vectors
### One of the biggest (and most successful) threat vectors
- everyone has at least one of these messaging system
### Email
- malicious links in an email
- link to malicious site
### SMS (Short Message Service)
- attacks in a text message
### Phishing attacks
- people want to click links
- links in an email, links send via text or IM
### Deliver the malware to the user
- attach to email
- scan all attachments, never launch untrusted links
### Social engineering attacks
- invoice scams
- cryptocurrency scams
# Image-based vectors
### Easy to identify a text-based threat
- it's more difficult to identify the threat in an image
### Some image formats can be a threat
- the SVG format (Scalable Vector Graphics)
- image is describe in XML (Extensible Markup Language)
### Significant security concerns
- HTML injection
- JavaScript attack code
### Browsers must provide input validation
- avoids running malicious code
# File-based vectors
### More than just executables
- malicious code can hide in many places
### Adobe PDF
- a file format containing other objects
### ZIP/RAR files (or any compression types)
- contains many different files
### Microsoft Office
- documents with macros
- add-in files
# Voice call vectors
### Vishing
- phishing over the phone
### Spam over IP
- large-scale phone calls
### War dialing
- it still happens
### Call tampering
- disrupting voice calls
# Removable device vectors
### Get around the firewall
- the USB interface
### Malicious software on USB flash drives
- infect air gapped networks
- industrial systems, high-security services
### USB devices can act as keyboards
- hack on a chip
### Data exfil
- TB of data walk out the door
- zero bandwidth used
# Vulnerable software vendors
### Client-based
- infected executable
- known (or unknown) vulnerabilities
- may require constant updates
### Agentless
- no installed executable
- compromised software on the server would affect all users
- client runs a new instance each time
# Unsupported systems vectors
### Patching is an important prevention tool
- ongoing security fixes
### Unsupported systems aren't patched
- there may not even be an option
### Outdated operating system
- eventually, even the manufacturer won't help
### A single system could be an entry
- keep your inventory and records current
# Unsecure network vectors
### The network connects everything
- ease of access for the attackers
- view all (non-encrypted) data
### Wireless
- outdated security protocols (WEP,WPA,WPA2)
- open or rogue wireless networks
### Wired
- unsecure interfaces - no 802.1X
### Bluetooth
- reconnaissance
- implementation vulnerabilities
# Open service ports
### Most network-based services connect over TCP/UDP port
- an "open" port
### Every open port is opportunity for attacks
- app vuln or misconfig
### Every app has their own open port
- more services expand the attack surface
### Firewall rules
- must allow traffic to an open port
# Default credentials
### Most devices have default user and passwords
- change yours
### The right cred provide full control
- admin access
### Very easy to find default creds for AP or router
- https://www.routerpasswords.com
# Supply chain vectors
### Tamper with the underlying infra
- or manufacturing process
### Managed service providers (MSPs)
- access many different customer networks from one location
### Gain access to a network using a vendor
- 2013 target credit card breach
### Suppliers
- counterfeit networking equipment
- install backdoors, substandard performance and availability
- 2020 - Fake Cisco Catalyst switches