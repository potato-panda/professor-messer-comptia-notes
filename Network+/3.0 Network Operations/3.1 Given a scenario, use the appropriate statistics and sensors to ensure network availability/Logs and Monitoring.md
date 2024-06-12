# Traffic logs
### View traffic information from routers, switches, firewalls, etc
- identify traffic flows
- view traffic summaries
### Can be very detailed
- every flow from every devices
### Important historical information
- monitoring, post-event analysis
![[Pasted image 20240513165429.png]]
# Audit logs
### What did they do, and when did they do it?
- often more specific than general traffic logs
![[Pasted image 20240513165537.png]]
# Syslog
### Standard for message logging
- diverse systems create a consolidated log
### Usually a central logging receiver
- integrated into the SIEM (Security Information and Event Manager)
### Each log entry is labeled
- facility code (program that create the log) and severity level
# Severity levels
### Not all alerts have the same priority
- low level debug and information
- high level critical and alert
### Alerts can be used as a filter
- only show Warning level and higher
### You decide the importance of each alert level
- information may or may not be useful
![[Pasted image 20240513165848.png]]
# Interface errors
### Runts
- frames that are less than 64 bytes (minimum size of Ethernet frame is 64 bytes)
- may be a result of a collision
### Giants
- frames that are more than 1518 bytes
### CRC error (Cyclical Redundancy Check)
- failed the Frame Check Sequence (FCS error)
- may indicate a bad cable or interface
### Encapsulation error
- inconsistent configurations between switches - ISL (Inner Switch Link) or 802.1Q
![[Pasted image 20240513170301.png]]
# Environmental sensors
### Temperature
- devices need constant cooling
- so do humans
### Humidity level
- high humidity promotes condensation
- low humidity promotes static discharges
### Electrical
- device and circuit load
### Flooding
- water and electrical devices don't get along
# Baseline review
![[Pasted image 20240513170533.png]]
# NetFlow
### Gather traffic statistics from all traffic flows
- shared communication between devices
### NetFlow
- standard collection method
- many products and options
### Probe and collector
- probe watches network communication
- summary records are sent to the collector
# Usually a separate reporting app
- closely tied to the collector
![[Pasted image 20240513170621.png]]
![[Pasted image 20240513170735.png]]
![[Pasted image 20240513170744.png]]
# Uptime and downtime
### Is it up or down?
- it can often be difficult to tell
### Uptime and downtime status page
- a summary of availability
- you know they know
![[Pasted image 20240513170851.png]]