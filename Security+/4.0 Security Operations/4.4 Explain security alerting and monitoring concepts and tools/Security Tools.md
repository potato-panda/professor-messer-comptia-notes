# Security Content Automation Protocol (SCAP)
### Many different security tools in market
- NGFWs, IPS, vuln scanners, etc
- all have own method of evaluating threats
### Managed by NIST
- https://scap.nist.gov/
### Allows tools to ID and act on same criteria
- validate security config
- confirm patch installs
- scan for security breaches
# Using SCAP
### SCAP content can be shared between tools
- focused on config compliance
- easily detect apps with known vulns
### Esp. useful in large env
- many diff OS and apps
### This spec standard enables automation
- even between tools
### Automation types
- ongoing monitoring
- notif and alerting
- remediation of noncompliant systems
# Benchmarks
### apply security best-practices to everything
- OS, cloud, providers, mobile devices, etc
- bare minimum for security settings
### Example: Mobile device
- disable screenshots, disable screen recordings, prevent voice calls when locked, force encryption backups, disable additional VPN profiles, configure a "lost phone" message, etc
### Popular benchmarks - Center for Internet Security (CIS)
- https://www.cisecurity.org/cis-benchmarks/
# Agents/agentless
### Check to see if device is in compliance
- install a software agent onto device
- run an on-demand agentless check
### Agent can usually provide more detail
- always monitoring for real-time notif
- must be maintained and updated
### Agentless runs without a formal install
- performs a check, then disappears
- does not required ongoing updates to an agent
- will not inform or alert if not running
# [[Study/professor-messer-comptia-notes/Network+/4.1/Risk Management#SIEM|SIEM]]
# Anti-virus/Anti-malware
### Anti-virus is the popular term
- refers specifically to a type of malware
- Trojans, worms, macro viruses
### Malware refers to the broad malicious software category
- anti-malware stops spyware, ransomware, fileless malware
### The terms are effectively the same these days
- the names are more of a marketing tool
- anti-virus software is also anti-malware software now
- make sure your system is using a comprehensive solution
# [[Study/professor-messer-comptia-notes/Network+/3.2/Security Policies#Data Loss Prevention (DLP)|Data Loss Prevention (DLP)]]
### Stop data before attacker gets it
- data "leakage"
### So many sources, so many destinations
- often requires multiple solutions
- endpoint clients
- cloud-based systems
	- email, cloud storage, collab tools
# [[SNMP]]
### Request statistics from a device
- server, firewall, workstation, switch, router, etc
### Poll devices at fixed intervals
- create historical performance graphs
### Graphing
![[Pasted image 20240610143731.png]]
# SNMP traps
### Most SNMP operations expect a poll
- devices then respond to the SNMP request
- this requires constant polling
### SNMP traps can be configured on the monitored device
- comms over udp/162
### Set a threshold for alerts
- if number of CRC errors increases by 5, send a trap
- monitoring station can react immediately
# [[Logs and Monitoring#NetFlow|NetFlow]]
# Vulnerability scanners
# [[Vulnerability Scanning#Vulnerability scanners|Vulnerability scanners]]