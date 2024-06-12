# Segmenting the network
### Physical, logical, or virtual segmentation
- devices, VLANs, virtual networks
### Performance
- high-bandwidth apps
### Security
- users should not talk directly to db servers
- only apps in the core are SQL and SSH
### Compliance
- mandated segmentation (PCI compliance)
- makes change control much easier
# [[Network Hardening#Access Control lists (ACLs)|Access control lists (ACLs)]]
### List the permissions
- Bob can read files
- Fred can access the network
- James can access network 192.168.1.0/24 using TCP ports 80, 443, and 8088
### Many OS uses ACLs to provide access to files
- a trustee and the access rights allowed
# [[Technical Change Management#Allow list / deny list|Application allow / deny list]]
### Decisions are made in the OS
- often built-in to the OS mgnt
### Application hash
- only allows apps with this unique ID
### Certificate
- allow digitally signed apps from certain publishers
### Path
- only run apps in these folders
### Network zone
- the apps can only run from this network zone