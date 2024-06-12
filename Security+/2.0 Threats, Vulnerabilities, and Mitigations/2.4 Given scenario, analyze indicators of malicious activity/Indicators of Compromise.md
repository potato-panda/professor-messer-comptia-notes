# Indicators of Compromise (IoC)
### Event that indicates an intrusion
- confidence is high
- calling inside the house
### Indicators
- unusual amount of network activity
- change to file hash values
- irregular international traffic
- changed to DNS data
- uncommon login patterns
- spikes of read requests to certain files
# Account lockout
### Creds are not working
- it wasn't you this time
### Exceeded login attempts
- account is automatically locked
### Account was admin disabled
- this would be larger concern
### This may be a part of a larger plan
- attacker locks account
- calls support line to reset the password
# Concurrent session usage
### It's challenging to be two places at one time
- laws of physics
### Multiple account logins from multiple locations
- interactive access from a single user
- you don't have a clone
### This can be difficult to track down
- multiple devices and desktops
- automated processes
# Blocked content
### Attacker wants to stay as long as possible
- your system has been unlocked
- keep the doors and windows open
### There's probably a security patch available
- time to play keep-away
### Blocked content
- auto-update connections
- links to security patches
- third-party anti-malware sites
- removal tools
# Impossible travel
### Auth logs can be telling
- logon and off
### Login from Omaha, Nebraska, US
- the company HQ
### 3 mins later, a login from Melbourne, Victoria, Australia
- alarms should be ringing
### This should be easy to ID
- log analysis and automation
# Resource consumption
### Every attackers, action has an equal and opposite reaction
- watch carefully for significant changes
### File transfer use bandwidth
- an unusual spike at 3AM
### Firewall logs show the outgoing transfer
- IP addresses, timeframes
### Often the first real notif of an issue
- attacker may have been there for months
# Resource inaccessibility
### The server is down
- not responding
### Network disruption
- cover for the actual exploit
### Server outage
- result of an exploit gone wrong
### Encrypted data
- potential ransomware attack begins
### Brute force attacks
- locks account access
# Out-of-cycle logging
### Out-of-cycle
- occurs at an unexpected time
### OS patch logs
- occurring outside of normal patch day
- keep that exploited system safe from other attackers
### Firewall log activity
- timestamps of every traffic flow
- protocols and apps used
# Missing logs
### Log info is evidence
- attackers will try to cover their tracks be removing logs
### Info is everywhere
- auth logs
- file access logs
- firewall logs
- proxy logs
- server logs
### The logs may be incriminating
- missing logs are certainly suspicious
- logs should be secure and monitored
# Published / documented
### The entire attack and data exfil may go unnoticed
- it happens quite often
### Company data may be published online
- attackers post a portion or all data
- may be conjunction with ransomware
### Raw data may be release without context
- researchers will try to find the source