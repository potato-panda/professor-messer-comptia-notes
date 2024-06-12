# Designing the Cloud
### On-demand computing power
- with a click of a button 
### Elasticity
- scale up or down as needed
### Applications also scale
- scalability for large implementations
- access from anywhere
### Multitenancy
- many different clients are using the same cloud architecture
# Infrastructure as code
### Describe an infrastructure
- define servers, network, and applications as code
### Modify the infrastructure and create versions
- the same way you version application code
### Use the description (code) to build other application instances
- build it the same way every time based on the code
### An important concept for cloud computing
- build a perfect version every time
![[Pasted image 20240509163837.png]]
# Orchestration
### Automation is the key to cloud computing
- services appear and disappear automatically, or at the push of a button
### Entire application instances can be instantly provisioned
- all servers, networks, switches, firewalls, and policies
### Instances can move around the world as needed
- follow the sun
### The security policies should be part of the orchestration
- as applications are provisioned, the proper security is automatically included
# Connecting to the cloud
### VPN
- site-to-site virtual private network
- encrypt through the internet
### Virtual Private Cloud Gateway
- connects users on the Internet
### VPC Endpoint
- direct connection between cloud provider networks
![[Pasted image 20240509164135.png]]
# Virtual private cloud endpoints
![[Pasted image 20240509164225.png]]
# VM sprawl avoidance
### Click a button
- you've built a server
- or multiple servers, networks, and firewalls
### It becomes almost too easy to build instances
- this can get out of control quickly
### The virtual machines are sprawled everywhere
- you aren't sure which VMs are related to which applications
- it becomes extremely difficult to deprovision
### Formal process and detailed documentation
- you should have information on every virtual object
  ![[Pasted image 20240509164743.png]]
# VM escape protection
### The VM is self-contained
- There's no way out?
- Or is there?
### Virtual machine escape
- break out of the VM and interact with the host operating system or hardware
### Once you escape the VM, you have great control
- control the host and control other guest VMs
### This would be a huge exploit
- full control of the virtual world
# Escaping the VM
### March 2017 - Pawn2Own competition
- hacking contest
- you pwn it, you own it - along with some cash
### JavaScript engine bug in Microsoft Edge
- code execution in the Edge sandbox
### Windows 10 kernel bug
- compromised the guest operating system
### Hardware simulation bug in VMware
- escape to the host - **CVE-2017-4901**
