# Threat assessment
### Research the threats
- and the threat actors
### Data is everywhere
- hacker group profiles, tools used by the attackers, and much more
### Make decisions based on this intelligence
- invest in the best prevention
### Used by researchers, security operation teams, and others
# Vulnerability assessment
### Usually minimally invasive
- unlike a pentest
### Run a vulnerability scanner
- poke around and see what's open
### Identify systems
- and security devices
### Test from the outside and inside
- don't dismiss insider threats
### Gather as much information as possible 
- we'll separate wheat from chaff later
# Vulnerability scan results
### Lack of security controls
- no firewall
- no AV
- no anti-spyware
### Misconfigurations
- open shares
- guest access
### Real vulnerabilities
- especially newer ones
- occasionally the old ones
# Penetration testing
### Pentest
- simulate an attack
### Similar to vulnerability scanning
- except we actually try to exploit the vulnerabilities
### Often a compliance mandates
- regular penetration testing by a 3rd-party
### Nation Institute of Standards and Technology Technical Guide to Information Security Testing and Assessment
- https://professormesser.link/800115 (PDF download)
# Posture assessment
### You can't trust everyone's computer
- BYOD
- Malware infections/ missing anti-malware
- unauthorized applications
### Before connecting to the network, perform a health check
- is it a trusted device?
- is it running AV? Which one? Is it updated?
- are there corporate applications installed?
- is it a mobile device? is the disk encrypted?
- the type of device doesn't matter - Windows, Mac, Linux, iOS, Android
# Failing your assessment
### What happens when a posture assessment fails?
- too dangerous to allow access
### Quarantine network, notify administrators
- just enough network access to fix the issue
### Once resolved, try again
- may require additional fixes
# Risk assessment
### Identify assets that could be affected by an attack
- define the risk associated with each asset
- hardware, customer data, intellectual property
### Identify threats
- loss of data, disruption of services, etc
### Determine the risk
- high, medium, or low risk
### Process assessment
- make future security plans
# Vendors
### Every organization works with vendors
- payroll, customer relationship management, email marketing, travel, raw materials
### Important company data is often shared
- may be required for cloud-based services
### Perform a risk assessment
- categorize risk by vendor and manage the risk
### Use contracts for clear understanding
- make sur everyone understand the expectations
- use the contract to enforce a secure environment
# SIEM
### Security Information and Event Management
- logging of security events and information
### Security alerts
- real-time information
### Log aggregation and long-term storage
- usually includes advanced reporting features
### Data correlation
- link diverse data types
### Forensic analysis
- gather details after an event
# Getting the data
### Sensors and logs
- operating systems
- infrastructure devices
- NetFlow sensors
### Sensitively settings
- easy to be overwhelmed with data
- some information is unnecessary
- Informational, Warning, Urgent
![[Pasted image 20240513230215.png]]
# Viewing the data
### Trends
- identify changes over time
- easily view constant attack metrics
### Alerts
- identify a security event
- view raw data
-  visual the log information
### Correlation
- combine and compare
- view data in different ways