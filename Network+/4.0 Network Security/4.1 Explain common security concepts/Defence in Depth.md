# Layer the defence
### Physical controls
- keep people away from the technology
- door locks, fences, rack locks, cameras
### Technical controls
- hardware an software to keep things secure
- firewalls, active directory authentication, disk encryption
### Administrative controls
- policies and procedures
- onboarding and offboarding
- backup media handling
# Defence in depth
- Firewall
- Screened subnet (DMZ)
- Hashing and salting passwords
- Authentication
- Intrusion prevention system
- VPN access
- Card/badge access
- AV and Anti-Malware software
- Security Guard
# Physical segmentation
### Separate devices
- multiple units, separate infrastructure
![[Pasted image 20240513222012.png]]
# Logical segmentation with VLANs
### Virtual LANs
- separated logically instead of physically
- cannot communication between VLANs without a Layer 3 device/router
![[Pasted image 20240513222122.png]]
# Screened subnet
### Previously known as the demilitarized zone (DMZ)
- an additional layer of security between the Internet and you
- public access to public resources
![[Pasted image 20240513222233.png]]
# Separation of duties
### Split knowledge
- no one person has all of the details
- half of a safe combination
### Dual control
- two people must be present to perform the business function
- two keys open a safe (launch a missile)
# Network Access Control (NAC)
### IEEE 802.1X - Port-based Network Access Control 
- you don't get access until you authenticate
### We're talking about physical interfaces
- not TCP or UDP ports
### Makes extensive use of EAP  and RADIUS
- Extensible Authentication Protocol / Remote Authentication Dial in User service
### Administrative enable/disable
- disable your unused ports
### Duplicate MAC address checking
- stop the spoofers
# IEEE 802.1X
![[Pasted image 20240513222739.png]]
![[Pasted image 20240513222746.png]]
![[Pasted image 20240513222752.png]]
![[Pasted image 20240513222759.png]]
![[Pasted image 20240513222805.png]]
![[Pasted image 20240513222811.png]]
![[Pasted image 20240513222823.png]]
![[Pasted image 20240513222828.png]]
![[Pasted image 20240513222839.png]]
# Honeypots
### Attract the bad guys
- and trap them there
### The "attacker" is probably a machine
- makes for interesting recon
### Honeypots
- creates a virtual world to explorer
### Many different options
- Kippo, Google Hack Honeypot, Wordpot, etc