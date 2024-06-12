# SAN
### Storage Area Network (SAN)
- looks and feels like a local storage drive
- block-level access
- very efficient reading and writing
### Requires a lot of bandwidth
- may use an isolated network and high-speed network technologies
# Fibre Channel (FC)
### A specialized high-speed topology
- connect servers to storage
- 2, 4, 8 and 16-gigabit/s rates
- supported over both fiber and copper
### Servers and storage connect to a Fibre Channel Switch
- server (initiator) needs a FC interface
- storage (target) is commonly referenced by SCSI, SAS, or SATA commands
# Fibre Channel over Ethernet (FCoE)
### Use Fibre Channel over Ethernet network
- no special networking hardware needed
- usually integrates with an existing FC infra
- nout routable
# iSCSI
### Internet Small Computer Systems Interface
- send SCSI commands over an IP network
- created by IBM and Cisco, now an RFC standard
### Makes a remote disk look and operate like a local disk
- like FC
### Can be managed quite well in software
- drivers available for many Operating systems
- no proprietary topologies or hardware needed