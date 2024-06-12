# A series of moving vans
### Efficiently move large amounts of data
- use a shipping truck
### The network topology is the road
- Ethernet , DSL, cable system
### The truck is the Internet Protocol (IP)
- we've designed the roads for this truck
### The boxes hold your data 
- boxes of TDP and UDP
### Inside the boxes are more things
- application info
# IP - Internet Protocol
![[Pasted image 20240508115550.png]]
# TCP and UDP
### Transported inside of IP
- encapsulated by the IP
### Two ways to move data from place to place
-  different features for different applications
### OSI Layer 4
 - the transport layer
### Multiplexing
 - use many different applications at the same time
 - TCP and UDP
# TCP - Transmission Control Protocol
### Connection-orientated
- formal connection setup and close
### "Reliable" delivery
- recovery from errors
- can manage out-of-order messages or retransmissions
### Flow Control
- the receiver can manage how much data is sent
![[Pasted image 20240508115826.png]]

# UDP - User Datagram Protocol
### Connectionless
- no formal open or close to the connection
### "Unreliable" Delivery
- no error recovery
- no reordering of data or retransmissions
### No flow control
- sender determines amount of data transmitted

![[Pasted image 20240508115957.png]]

# Speedy delivery
### The IP delivery truck delivers from one IP address to another IP address
- every house has an address, every computer has an IP address
### Boxes arrive at the house/IP address
- where do the boxes go?
- each box has a room name
### Port is written on the outside of the box
- drop the box into the right room
# Lots of ports
### IPv4 sockets
- server IP address, protocol, server app port number
- client IP address, protocol, client port number
### Non-ephemeral ports - permanent port numbers
- ports 0 through 1023
- usually on a server or service
### Ephemeral ports - temporary port numbers
- ports 1024 through 65535
# Port Numbers

### TCP and UDP ports can be any number between 0 and 65535
### Most servers/services use non-ephemeral (temporary) port numbers
- it's not always the case
	- it's just an arbitrary chosen port number
### Ports numbers are for communication, not security
### Service port numbers need to be "well known"
### TCP port numbers aren't the same as UDP port numbers
# Ports on the network
### Web server - TCP/80
### VoIP server - UDP/5004
### Email server - TCP/143

![[Pasted image 20240508124921.png]]
