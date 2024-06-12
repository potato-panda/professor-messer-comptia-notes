# Hub
### Multi-port repeater
- traffic going in one port is repeated to every other port
- OSI layer 1
### Everything is half-duplex
> Either send or receive data, not both
### Becomes less efficient as network traffic increases
###  10/100 megabit/s
### Difficult to find today
> We use switches instead of Hubs today
# Bridge
### Image a switch with two to four ports
- makes forwarding decisions in software
### Connect different physical networks
- can connect different topology
- gets around physical network size limitations/collisions
### OSI Layer 2 device
- distributes traffic based on MAC address
### Example of a modern bridge is a wireless access point
- bridges wired Ethernet to wireless
# Switch
### Bridging done in hardware
- application-specific integrated circuit (ASIC)
### OSI Layer 2 devices
- forwards traffic based on data link address
### Many ports and features
- the core of an enterprise network
- may provide Power over Ethernet (PoE)
### Multilayer switch
- includes Layer 3 (routing) functionality
# Router
### Routes traffic between IP subnets
- OSI Layer 3 device
- Routers inside of switches sometimes called "Layer 3 switches"
- Layer 2 = Switch, Layer 3 = Router
### Commonly connects diverse network types
- LAN, wan, Copper, fiber
# Access point
### Not a wireless router
- a wireless router is a router and an access point in a single device
### An access point is a bridge
- extends the wired network onto the wireless network
- OSI Layer 2 device
# Cable modem
### Broadband
- transmission across multiple freq
- different traffic types
### Data on the "cable" network
- DOCSIS (Data Over Cable Service Interface Specification)
### High-speed networking
- 4 to 250 M/bits are common
- Gigabit speeds are possible
### Multiple servers
- Data, voice, video
# DSL modem
### ADSL (Asymmetric Digital Subscriber Line)
- uses existing telephone lines
### Download speeds are faster than upload speeds (asymmetric)
- 10,000 foot limitation from the central office (CO)
- 52Mb/s down / 16Mb/s up are common
- Better speeds are possible if closer to CO
# Repeater
### Receive signal, regenerate, resend
- no forwarding decisions to make
### Common uses
- boost copper or fiber connections
- convert one network media to another
- extend wireless network reach
# Converting media
### OSI layer 1
- physical layer signal conversion
### Extend a copper wire over a long distance
- convert it to fiber and back again
### You have fiber
- the switch only has copper ports
### Almost always powered
- especially fiber to copper