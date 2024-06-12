# Three-tier architecture
### Core
- the 'center' of the network
- web servers, databases, applications
- many people need access to this
### Distribution
- a midpoint between the core and the users
- communication between access switches
- manages the path to the end users
### Access
- where the users connect
- end stations, printers
![[Pasted image 20240509145724.png]]
> Downtown is the core
![[Pasted image 20240509145801.png]]
> Core at the bottom

# SDN (Software Defined Networking)
### Networking devices have different functional planes of operation
- data, control, and management planes
### Split the functions into separate logical units
- extends the functionality and management of a single device
- perfectly built for the cloud
### Infrastructure layer/ Data plane
- process the network frames and packets
- does forwarding, trunking, encrypting, NAT
### Control layer / Control plane
- manages the actions of the data plane
- routing tables, session tables, NAT tables
- dynamic routing protocol updates
### Application layer / Management plane
- configure and manage the device
# Extend the physical architecture
![[Pasted image 20240509150429.png]]
# SDN data flows
![[Pasted image 20240509150456.png]]
# Spine and leaf architecture
### Each leaf switch connects to each spine switch
- each spine switch connects to each leaf switch
### Leaf switches do not connect to each other
- same for spine switches
### Top-of-rack switching
- each leaf is on the 'top' of a physical network rack
- may include a group of physical racks
### Advantages
- simple cabling
- redundant
- fast
### Disadvantages
- additional switches may be costly
![[Pasted image 20240509150654.png]]
# Traffic flows
### Traffic flows within a data center
- important to know where the traffic starts and ends
### East-west
- traffic between devices in the same data center
- relatively fast response times
### North-south traffic
- ingress/egress to an outside device
- a different security posture than east-west traffic
![[Pasted image 20240509150900.png]]
# Network locations
### Branch office
- a remote location
- client devices, printers, switch/router/firewall
### On-premises data center
- technology is located in-house
- requires power, cooling, and ongoing monitoring
### Colocation
- share a data center with others
- local oversight and monitoring