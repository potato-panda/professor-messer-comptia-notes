# Peer-to-peer (P2P)
- all devices are both clients and servers
	- everyone talks to everyone
### Pros
- easy to deploy
- low cost
### Cons
- hard to administer
- hard to secure
![[P2P.png]]

# Client-server
### Central server
- clients talk to server
### No client to client communication
### Pros
- performance and administration
### Cons
- cost and complexity
![[Client-server.png]]

# Local Area Network (LAN)
- local is relative
### A building or group of buildings
- high-speed connectivity
### Ethernet and 802.11 wireless
- any slower and it isn't 'local'

# Metropolitan Area Network (MANs)
- a network in your city
- larger than LAN and often smaller than a WAN
### Historically MAN-specific topologies
- everyone's moving to **Metro Ethernet**
### Common to see government ownership
- they 'own' the right-of-way
	- easy to put fiber in the ground and connect all their remote locations

# Wide Area Network (WANs)
- spanning the globe
### Generally connects LANs across a distance
- generally much slower than the LAN
### Many different WAN technologies
- point-to-point serial, MPLS, etc...
- terrestrial and non-terrestrial
	- can be links connecting us to fiber in the ground
	- satellite are certainly a WAN and allow to connect to very remote networks
# Wireless Local Area Network (WLANs)
- 802.11 technologies
### Mobility
- within a building
- in a limited geographical area
### Expand coverage with additional access points
- downtown area
- large campus

# Personal Area Network (PAN)
- your own private network
- Bluetooth, IR, NFC
### Automobile
- audio output
- integrate with phone
### Mobile phone
- wireless headset
### Health
- workout telemetry, daily reports

# Campus Area Network (CAN)
- Corporate Area Network
### Limited geographical area
- a group of buildings
### LAN technologies
- fiber connection
- high-speed Ethernet
### Your own fiber in the ground
- no third-party provider

# Network Attached Storage vs Storage Area Network
### Network Attached Storage (NAS)
- connect to a shared storage device across the network
- **file-level access**
### Storage Area Network (SAN)
- looks and feels like a local storage devices
	- **block-level access**
- very efficient reading and writing
### Requires a lot of bandwidth
- may use an isolated network and high-speed network technologies

# Multiprotocol Label Switching (MPLS)
### Learning from ATM and Frame Relay
- keep advantages and solves disadvantages
### Communicates packets through the WAN, but have a label
- routing decisions are easy
### Any transport medium, any protocol inside
- IP packets, Ethernet frames
### A common WAN technology
- **Ready-to-network**
## MPLS pushing and popping
- Labels are "pushed" onto packets as they enter the MPLS cloud
- Labels are "popped" off on the way out
![[MPLS pushing and popping.png]]
## Multipoint Generic Router Encapsulation (mGRE)
- MPLS requires initial configuration defining where all the different sites may be located and what labels are used to switch data to those locations
- other types of WAN could create connections dynamically, so you're only connecting to those sites when needed; commonly using mGRE
- used extensively for Dynamic Multipoint VPN (DMVPN)
- common on Cisco routers
### Your VPN builds itself
- DMVPN sends data across one of the mGRE networks
- created only when needed; torn down when there's no information to send
- rebuilds itself when there is a break in any of the connection, to communicate with any of the different sites
- remote sites communicate with each other
### Tunnels are built dynamically on-demand
- **A dynamic mesh**: all considered to be a mesh because you're able to send data to whatever site based on where it needs to go 
# Software Defined Networking in a Wide Area Network (SD-WAN)
- defined arbitrary
- WAN built for the cloud
### The data center used to be in one places
- the cloud changed everything
### Cloud-based applications communicate directly to the cloud
- No need to hop through a central point
![[Pasted image 20240607152005.png]]
![[Pasted image 20240607152023.png]]
![[Pasted image 20240607152044.png]]