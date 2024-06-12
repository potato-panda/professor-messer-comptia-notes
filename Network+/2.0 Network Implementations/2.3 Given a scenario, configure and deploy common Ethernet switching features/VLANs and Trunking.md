# LANs
![[Pasted image 20240510194357.png]]
### Local Area Networks
- a group of devices in the same broadcast domain
# Virtual LANs
### Virtual Local Area Networks
- a group of devices in the same broadcast domain
- separated logically instead of physically
# Configuring VLANs
![[Pasted image 20240510194631.png]]
# VLANs on multiple switches
![[Pasted image 20240510194724.png]]
# VLAN trunking
![[Pasted image 20240510194818.png]]
# 802.1Q trunking
### Take a normal Ethernet frame
### Add a VLAN header in the frame
### VLAN IDs - 12 bits long, 4094 VLANs
- "normal range" from 1 to 1005, "extended range" from 1006 to 4094
- 0 and 4095 are reserved VLAN numbers
### Before 802.1Q, there was ISL (Inter-Switch Link)
- ISL is no longer used; everyone now uses the 802.1Q standard
  ![[Pasted image 20240510195138.png]]
# Trunking between switches
![[Pasted image 20240510195310.png]]
# Working with data and voice
### Old school: connect computer to switch, connect phone to PBX (Phone Branch Exchange)
- two physical cables, two different technologies
### Now: Voice over IP (VoIP)
- connect all devices to the Ethernet switch
- one network cable for both
# Data and voice cabling
### Computer connects to phone
### Phone connects to switch
### One cable, one run
![[Pasted image 20240510195511.png]]
# Just one problem
### Voice and data don't like each other
- voice is very sensitive to congestion
- data loves to congest the network
### Put the computer on one VLAN and the phone on another
- but the switch interface is not a trunk
- so how does that work?
### Each switch interface has a data VLAN and a voice VLAN
- configure each of them separately
# Configure voice and data VLANs
### Data passes as a normal untagged access VLAN
### Voice is tagged with an 802.1Q header
![[Pasted image 20240510195745.png]]