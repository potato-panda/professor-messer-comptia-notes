### No system is secure using default configs
- you need some guideless to keep everything safe
### Hardening guides are specific to the software or platform
- get feedback from the manufacturer or Internet interest group
- they'll have the best details
### Other general-purpose guides are available online
# Mobile devices
### Always-connected mobile technologies
- phones, tablets, etc
- hardening checklist are available from manufacturers
### Updates are critical
- bug fixes and security patches
- prevent known vulns
### Segmentation can protect data
- company and user data are separated
### Control with MDM (Mobile Device Manager)
# Workstation
### User desktops and laptops
- all OS
### Constant monitoring and updates
- OS, apps, firmware, etc
### Automate monthly patches
- there's likely an existing process
### Connect to a policy management system
- Active Directory group policy
### Remove unnecessary software
- limit the threats
# Network infrastructure devices
### Switches, routers, etc
- you never see them, but they're always there
### Purpose-built devices
- embedded OS, limited OS access
### Configure auth
- don't use defaults
### Check with manufacturer
- security updates
- not usually updated frequently
- updates are usually important
# Cloud infrastructure
### Secure the cloud management workstation
- keys to the kingdom
### Least privileges
- all services, network settings, app rights and permissions
### Configure Endpoint Detection and Response (EDR)
- all devices accessing the could should be secure
### Always have backups
- Cloud-to-cloud (C2C)
# [[Hardening Techniques#System hardening|Servers]]
# [[Networked Devices#SCADA / ICS|SCADA / ICS]]
# [[Other Infrastructure Concepts#Embedded systems|Embedded systems]]
### Can be difficult to upgrade
- watches and TVs are relatively easy
- other devices may not be easily modified
### Correct vulns
- security patches remove potential threats
### Segment and firewall
- prevent access from unauthd users
# [[Other Infrastructure Concepts#RTOS (Real-Time Operating System)| RTOS]]
### Isolate the system
- prevent access from other areas
### Run with minimum services
- prevent potential for exploit
### Use secure comms
- protect with host-based firewall
# [[Other Infrastructure Concepts#Networked Devices IoT (Internet of Things) devices IoT (Internet of Things)| IoT devices]]
### Deploy updates quickly
- can be significant security concern
### Segmentation
- put IoT devices on their own VLAN
