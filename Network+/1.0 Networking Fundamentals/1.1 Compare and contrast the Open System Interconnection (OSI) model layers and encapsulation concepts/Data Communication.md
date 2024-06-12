---
tags: 
aliases: how data is sent
---
# Protocol Data Unit (PDU)

- Transmission Units
	- a different group of data at different OSI Layers
- Ethernet operates on a frame of data
	- it doesn't care about the content of data
- IP operates on a packet of data
	- inside is TCP or UPD, again, content is irrelevant 
- TCP or UDP
	- TCP segment
	- UDP datagram

# Encapsulation and decapsulation

From a source (example)
1. Layers 5,6,7, Application Layer, produce application data
2. Layer 4, Transport, adds a TCP Header
3. Layer 3, Network, adds an IP Header
4. Layer 2, Data Link, wraps the data with a Frame Header and Frame Trailer
5. Sent through Layer 1, Physical, to the destination
6. Layer 2, Data Link, unwraps the data removing the Frame Header and Frame Trailer
7. Layer 3, Network, takes the IP Header
8. Layer 4, Transport, takes the TCP Header
9. Layer 5, Application, the data is received by the application to display to the user
![[Encapsulating data.png]]
![[Encapsulate and Decapsulate.png]]

# Dissecting a frame
- Each layer has a header and payload:
- Layer 2: MAC
	- Layer 3: IP
		- Layer 4: TCP/UDP
			- Layers 5-7: HTTPS, IMAP, SSH
![[Dissecting a frame.png]]

# TCP flags
- header describes/identifies the payload
- the TCP header contains important control information
	- includes a set of bits called TCP flags
- the flags control the payload
	- SYN: synchronize sequence numbers
	- PSH: push the data to application without buffering
	- RST: reset the connection
	- FIN: last packet from sender
![[TCP Flags.png]]

# Maximum Transmission Unit (MTU)
- maximum size IP packet to transmit
	- but not fragment
- fragmentation slows things down
	- losing a fragment loses the entire packet
	- requires overhead along the path
- hard to know the MTU all entire way through the path
	- automated methods are often inaccurate; especially when ICMP is filtered
![[MTU.png]]

# Building an Ethernet frame
![[Building an Ethernet frame.png]]

# What is IP fragmentation?
TCP Header + TCP Data can be seen here split into 3 fragments containing up to 16 bytes each
![[What is IP fragmentation.png]]

# Troubleshooting MTU
- MTU are usually configured once
	- based on the network infra and don't change often
- significant concern for tunnel traffic
	- as the tunnel may be smaller than your local Ethernet segment
- what if you send packets with Don't Fragment (DF) set?
	- Routers will respond back and tell you to fragment
	- or hope you get the ICMP message
- troubleshoot using 'ping'
	- ping with DF and force a maximum size of 1472 bytes
		- 1500 bytes - 8 byte ICMP header - 20 bytes IP address = 1472 
	- Windows: ping -f -l 1472 8.8.8.8
	- Linux and macOS: ping -D -s 1472 8.8.8.8