# Virtualization security
### Quite different than non-virtual machines
- can appear anywhere
### Quantity of resources vary between VMs
- CPU, memory, storage
### Many similarities to physical machines
- complexity adds opportunity for attackers
### Virtualization vulnerabilities
- local privilege escalations
- command ingjection
- info disclosure
# VM escape protection
### The VM is self-contained
- there's no way out
- or is there?
### VM escape
- break out of the VM and interact with host OS or hardware
### Once you escape VM, you have great control
- control the host and other guest VMs
### Huge exploit
- full control of the virtual world
# Escaping the VM
### March 2017 - Pwn2Own competition
- hacking contest
- you pwn it, you own it = along with some cash
### JavaScript engine bug in Microsoft Edge
- code execution in the Edge sandbox
### Windows 10 kernel bug
- compromise the guest OS
### Hardware simulation bug in VMware
- escape to the host
### Patches were release soon afterwards
# Resource reuse
### The hypervisor manages the relationship between physical and virtual resources
- available RAM, storage, CPU availability, etc
### These resources can be reused between VMs
- hypervisor hosts with 4GB of RAM
- supports 3 VMs with 2GB of RAM each
- RAM is allocated and shared between VMs
### Data can inadvertently be shared between VMs
- time to update the memory mgnt features
- security patches can mitigate risk