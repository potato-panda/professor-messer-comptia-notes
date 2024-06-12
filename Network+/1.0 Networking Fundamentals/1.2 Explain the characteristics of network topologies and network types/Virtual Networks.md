# Virtual Networks
### Used to have Server farms with 100+ individual computers
- it's a big farm
### All servers are connected with enterprise switches and routers
- With redundancy
### Migrate 100 physical servers to one physical server
- With 100 virtual servers inside
### What happens to the network then?

# Network functions virtualization (NFV)
### Replace physical network devices with virtual versions
- Managed from the hypervisor
### Same functionality as physical devices
- Routing, switching, load balancing, firewalls, etc.
### Quickly and easily deploy network functions as they are virtual, not physical
- Click and deploy from hypervisor
### Many deployment options
- VM, container, fault tolerance, etc..

# Hypervisor
### Virtual Machine Manager (VMM)
- Manages the virtual platform and quest OS
### Hardware management
- CPU
- Networking
- Security
-###Single console control
	- One pane of glass
# vSwitch
### Virtual switch
- Move the physical switch to virtual env
### Function is similar to physical
- Forwarding options
- Link aggregation
- Port mirroring
- NetFlow
### Deploy from hypervisor
- Automate with orchestration

# Virtual Network Interface Card (vNIC)
### VMs need a network interface
### Configured and connected through Hypervisor
- Enable additional features
- VLAN, aggregation, multiple interfaces
(Uplinks are interfaces that get information from virtual environment to physical world)