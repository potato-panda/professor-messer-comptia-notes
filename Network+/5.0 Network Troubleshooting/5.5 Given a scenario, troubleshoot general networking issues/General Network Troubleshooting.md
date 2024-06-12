# Device configuration review
### Don't start blindly troubleshooting
- know what you're getting into
### View the configuration
- native desktop or web-based console
- SSH/terminal console
### Try getting the configuration ahead of time
- prepare early
![[Pasted image 20240516155815.png]]
# Routing tables
### The digital version of asking for directions
- know how to get from point A to point B
### This can answer a lot of questions
- default gateway
- manually configured static routes
### Know which way data will flow
- a network map might help
### Refer to every router
- routing loops and missing routes are common
![[Pasted image 20240516160051.png]]
![[Pasted image 20240516160239.png]]
# Interface status
### Know the details of the important interfaces
- easy to view on the console
- you'll rarely be physically next to the device
### Check the easy stuff first
- verify the physical connectivity
- nothing works properly if the interface is misconfigured
### You will often solve the problem here
- check for errors and mismatches
- it's a quick and easy fix
![[Pasted image 20240516160432.png]]
![[Pasted image 20240516160445.png]]
![[Pasted image 20240516160453.png]]
# VLAN assignment
### Network link is active and IP address is assigned
- no access to resources or limit functionality
### Every switch interface is configured as an access port or a trunk port
- each access port is assigned to a VLAN
### Confirm the specific switch interface
- check the VLAN assignment
### This is also a common issue
- another quick fix
![[Pasted image 20240516160749.png]]
# Network performance baseline
### Troubleshooting starts with a blank state
- a baseline can add context
### Intermittent or all-day issues
- check utilization, individual device performance, etc
### Some organizations already collect this data
- check the SIEM or management console
### Look for patterns and correlation
- the baseline might also tell you what's NOT happening