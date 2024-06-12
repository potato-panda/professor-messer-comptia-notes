# ICMP
### Internet Control Message Protocol
- "text messaging" for your network devices
### Another protocol carried by IP
- not used for data transfer
### Devices can request and reply to admin requests
- Hey are you there, Yes I'm right here
### Devices can send message when thing don't go well
- that network you're trying to reach is not reachable from here
- Your Time to live expired, just letting you know
# GRE
### generic routing encapsulation
- the "tunnel" between two endpoints
### Encapsulate traffic inside of IP
- two endpoints appear to be directly connected to each other
- no built-in encryption
# VPNs
### Virtual Private Networks
- encrypted (private) data traversing a public network
### Concentrator
- encryption/decryption access devices
- often integrated in the firewall
### Many deployment options
- specialized cryptographic hardware
- software-based options available
### Used with client software
- sometimes built into the OS
# IPSec (Internet Protocol Security)
### Security for OSI Layer 3
- authentication and encryption for every packet
###  Confidentiality and integrity / anti-replay
- encryption and packet signing
### Very standardized
- common-to-use multi-vendor implementations
### Two core IPSec protocols
- Authentication Header (AH)
- Encapsulation Security Payload (ESP)
# Transport mode and tunnel mode
![[Pasted image 20240508152357.png]]
# Authentication Header (AH)
### Hash of the packet and a shared key
- MD5, SHA-1, SHA-2 are common
- adds the AH to the packet header
![[Pasted image 20240508152549.png]]
# Encapsulation Security Payload (ESP)
### Encrypts the packet
- MD5, SHA-1, SHA-2 for hash and 3DES or AES for encryptions
- adds a header, a trailer, and an Integrity Check Value
  ![[Pasted image 20240508152824.png]]
# IPSec Transport mode and Tunnel mode
  ![[Pasted image 20240508152926.png]]