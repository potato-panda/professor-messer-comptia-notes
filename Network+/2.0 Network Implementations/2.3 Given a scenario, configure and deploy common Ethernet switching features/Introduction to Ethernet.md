# SOHO LAN
![[Pasted image 20240510173909.png]]
# Enterprise network
![[Pasted image 20240510174606.png]]
> Core switches on the bottom floor
![[Pasted image 20240510174635.png]]
# The Ethernet frame
![[Pasted image 20240510174844.png]]
# The MAC address
### Ethernet Media Access Control address
- the 'physical' address of a network adapter
- unique to a device
### 48 bits / 6 bytes longs
- displayed in hexadecimal
![[Pasted image 20240510175426.png]]
# Duplex
### Half-duplex
- cannot send and receive simultaneously
- all LAN hubs are half-duplex devices
- switch interfaces can be configured as half-duplex
	- but usually only when connecting to other half-duplex devices
### Full-duplex
- data can be sent and received at the same time
- a properly configured switch interface will be set to full-duplex
# Half-duplex Ethernet
### Traffic received on one interface is repeated to all other interfaces
![[Pasted image 20240510175647.png]]
### If two devices communicate simultaneously, you have a collision
# CSMA/CD
### CS - Carrier Sense
- is there a carrier?
- is there a signal available that we can use to send some data?
### MA - Multiple Access
- more than one device on the network
### CD - Collision Detect
- Collision - two stations talking at once
- identify when data gets garbled
### Half-duplex Ethernet
- not used any longer
> Is a only a phenomenon in Half-duplex. Does not occur in Full-duplex
# CSMA/CD operation
### Listen for an opening
- don't transmit if the network is already busy
> will wait it's turn
### Send a frame of data
- you send data whenever you can
- there's no queue or prioritization
### If a collision occurs
- transmit a jam signal to let device know a collision has occurred
- wait a random amount of time
- retry the transmission
# Full-duplex Ethernet
### Sam's PC creates an Ethernet frame
- Sam's MAC is the source
- SGC server MAC address is the destination
### Frame is sent to Switch A
![[Pasted image 20240510180209.png]]
### Switch A examines the destination MAC address
- sends frame out the interface that matches the destination MAC
- device at the other end is Switch B
![[Pasted image 20240510180258.png]]
### Switch B forwards the frame to the interfaces that matches the destination (SGC server) MAC address
- destination PC receives the frame, identifies a matching destination MAC
- destination PC accepts the frame
![[Pasted image 20240510180347.png]]
### Full-duplex
- send and receive data simultaneously without collision