# System hardening
### Many and varied
- Any OS
### Updates
- OS updates / service packs, security patches
### User accounts
- minimum password lengths and complexity
- account limitations
### Network access and security
- limit network access
### Monitor and secure
- AV, anti-malware
# [[Mitigation Techniques#Encryption|Encryption]]
### Encrypt all network communication
- Virtual Private Networking (VPN)
- application encryption
# The endpoint
### The user's access
- applications and data
### Stop the attackers
- in/outbound attacks
### Many different platforms
### Protection is multi-faceted
- defence-in-depth
# Endpoint detection and response (EDR)
### A different method of threat protection
- scale to meet the increasing number of threats
### Detect a threat
- signature aren't the only detection tool
- behavioral analysis, ML, process monitoring
- lightweight agent on the endpoint
### Investigate the threat
- root cause analysis
### Respond to the threat
- isolate the system, quarantined the threat, rollback to a previous config
- API driven, no user or technician intervention required
# Host-based firewall
### Software-based firewall
- personal firewall, runs on every endpoint
### Allow/Disallow incoming/outgoing app traffic
- control by app process
- view all data
### ID and block unknown processes
- stop malware before it can start
### Manage centrally
# Finding intrusions
### Host-based Intrusion Prevention System (HIPS)
- recognize and block known attacks
- secure OK and app configs, validate incoming service requests
- often build into endpoint protection service
### HIPS identification
- signatures, heuristics, behavioral
- buffer overflows, registry updates, writing files to the Windows folder
- access to non-encrypted data
# Open ports and services
### Very open port is a possible entry point
- close everything except required ports
### Control access with a firewall
- NSFW would be ideal
### Unused or unknown services
- install with OS or from other apps
### Apps with broad port ranged
- open port 0 through 65,535
### Use Nmap or similar port scanner to verify
- ongoing monitoring is important
# Default password changes
### Every network device has a mgnt interface
- critical systems, other devices
### Many apps also have mgnt or maintenance interfaces
- can contain sensitive data
### Change default settings
- passwords
### Add additional security
- require additional logon
- add 3rd-party auth
# Removal of unnecessary software
### All software contains bugs
- some of the bugs are security vulnerabilities
### Every app seems to have a completely different patching process
- can be challenging to manage ongoing updates
### Remove all unused software
- reduce you risk
- an easy fix