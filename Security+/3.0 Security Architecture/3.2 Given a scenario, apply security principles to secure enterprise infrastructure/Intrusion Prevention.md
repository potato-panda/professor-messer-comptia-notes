# Intrusion Prevention System (IPS)
### Watch network traffic
### Intrusions
- exploits against OS, apps, etc
- buffer overflows, cross-site scripting, other vulnerabilities
### Detection vs Prevention
- Intrusion Detection System (IDS) - alarm or alert
- Prevention - stop it before it gets into the network
# Failure modes
### We hope for 100% uptime
- unrealistic
- something will break
### Fail-open
- when system fails, data continues to flow
### Fail-closed
- when system fails, data does not flow
# Device connections
### Active monitoring
- system is connected inline
- data can be blocked in real-time as it passes by
- intrusion prevention is commonly active
### Passive monitoring
- a copy of the network traffic is examined using a tap or port monitor
- data cannot be blocked in real-time
- intrusion detection is commonly passive
# Active monitoring
### IDS/IPS sits physically inline
- all traffic passes through the IDS/IPS
### Malicious traffic is immediately ID
- dropped at the IPS
- doesn't proceed through network
![[Pasted image 20240607134255.png]]
# Passive monitoring
### Examine a copy of the traffic
- port mirror (SPAN), network tap
### No way to block (prevent) traffic
- common with IDS
![[Pasted image 20240607134512.png]]
