# [[Hardening Techniques#The endpoint|The endpoint]]
# Edge vs. access control
### Control at the edge
- your Internet link
- managed primarily through firewall rules
- firewall rules rarely change
### Access control
- control from wherever you are
	- inside/outside
- access can be based on many rules
	- by user, group, location, app, etc
- access can be easily revoked/changed
	- change your security posture at any time
# [[Study/professor-messer-comptia-notes/Network+/4.1/Risk Management#Posture assessment|Posture assessment]]
# Health checks/posture assessment
### Persistent agents
- permanently installed onto a system
- periodic updates may be required
### Dissolvable agents
- no installation required
- runs during posture assessment
- terminates when no longer required
### Agentless NAC
- integrated with AD
- checks made during login/off
- can't be scheduled
# Failing assessment
### What happens?
- too dangerous to allow
### Quarantine network, notif admins
- just enough network access to fix the issues
### Once resolved, try again
- may require additional fixes
# [[Hardening Techniques#Endpoint detection and response (EDR)|EDR]]
# Extended Detection and Response (XDR)
### Evolution of EDR
- improve missed detections, false positives, and long investigation times
- attacks involve more than just the endpoint
### Add network-based detection
- investigate and respond to network anomalies
### Correlate endpoint, network, and cloud data
- improve detection rates
- simplify security event investigations
# User behaviour analytics
### XDR commonly includes user behaviour analytics
- extend scope of anomaly detection
### Watch users, hosts, network traffic, data repos, etc.
- create baseline or normal activity
- requires data analysis over an extended period
### Watch for unusual activity
- use a set of rules, pattern matching, statistical analysis
### Real-time detection of unusual activity
- catch threat early