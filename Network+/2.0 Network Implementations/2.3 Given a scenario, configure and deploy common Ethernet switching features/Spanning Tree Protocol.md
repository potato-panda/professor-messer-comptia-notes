# Loop protection
### Connect two switches to each other
- create a loop with two cables
- they'll send traffic back and forth forever
- there's no "counting" mechanism at the MAC layer
### This is an easy way to bring down a network
- and somewhat difficult to troubleshoot
- relatively easy to resolve
### IEEE standard 802.1D to prevent loops in bridged (switched) networks (1990)
- created by Radia Perlman
# STP port states
### Blocking
- not forwarding to prevent a loop
### Listening
- not forwarding and cleaning the MAC table
### Learning
- not forwarding and adding to the MAC TABLE
### Forwarding
- data passes through and is fully operational
### Disabled
- admin has turned off the port
# Spanning tree protocol
![[Pasted image 20240511003838.png]]
# RSTP (802.1w)
### Rapid Spanning Tree Protocol (802.1w)
- a much-needed update of STP
- this is the latest standard
### Faster convergence
- from 30 to 50 to 6 seconds
### Backwards compatible with 802.1D STP
- you can mix both in your network
### Very similar process
- an update, not a wholesale change