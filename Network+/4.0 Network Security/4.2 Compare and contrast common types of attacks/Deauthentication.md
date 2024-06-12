# It started as a normal day
### Surfing along on your wireless network
- and then you're not
### And then it happens again
- and again
### You may not be able to stop it
- there's (almost) nothing you can do
- time to get a long patch cable
### Wireless de-authentication
- a significant wireless denial of service (DoS) attack
# 802.11 management frames
### 802.11 wireless includes a number of management frames
- frames that make everything work
- you never see them
### Important for the operation of 802.11 wireless
- how to find access points, a mange QoS, associate/dissociate with an access point, etc
### Original wireless standards did not add protection for management frames
- sent in the clear
- no authentication or validation
![[Pasted image 20240514180541.png]]

https://youtu.be/-fh37E_H3wM?si=0t9ZLrhVZByvXcWv&t=92

# Protect against deauth attacks
### IEEE has already addressed the problem
- 802.11w - July 2014
### Some of the important management frames are encrypted
- disassociate, deauthenticate, channel switch announcements, etc
### Not everything is encrypted
- beacons, probes, authentication, association
### 802.11w is required for 802.11ac compliance
- this will continue to roll out going forward