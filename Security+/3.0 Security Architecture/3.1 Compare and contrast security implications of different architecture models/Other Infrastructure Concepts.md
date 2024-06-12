# Attacks can happen anywhere
### Two categories for IT security
- "On-premises data is more secure!"
- "Cloud-based data is more secure!"
### Cloud-based security is centralized and costs less
- no dedicated hardware, no data center to secure
- a third-party handles everything
### On-premises puts the security burden on the client
- data center security and infra costs
### Attackers want data
- regardless where it is
# On-premises security
### Customize you security posture
- full control when everything is in-house
### On-site IT team can manage security better
- local team can ensure everything is secure
- can be expensive and difficult to staff
### Local team maintains uptime and availability
- system checks can occur at any time
- no phone call for support
### Security changes can take time
- new equipment, configs, and additional costs
# Centralized vs decentralized
### Most orgs are physically decentralized
- many locations, cloud providers, OS, etc
### Difficult to manage and protect so many diverse systems
- centralize the security mgnt
### A centralized approach
- correlated alerts
- consolidated log file analysis
- comprehensive system status and maintenance/patching
### It's not perfect
- single point of failure, potential performance issues
# Virtualization
### Run many different OS on the same hardware
### Each app instance has it's own OS
- adds overhead and complexity
- virtualization is relatively expensive
![[Pasted image 20240607125739.png]]
# Application containerization
### Container
- contains everything you need to run an app
- code and dependencies
- a standardized unit of software
### Isolated processes in a sandbox
- self-contained
- apps can't interact with each other
### Container image
- a standard for portability
- lightweight, uses the host kernel
- secure separation between apps
![[Pasted image 20240607125903.png]]
# [[Networked Devices#IoT (Internet of Things) devices|IoT (Internet of Things)]]
### Sensors
- heating and cooling, lighting
### Smart devices
- home automation, video doorbells
### Wearable tech
- watches, health monitors
### Facility automation
- temps, air quality, lighting
### Weak defaults
- IoT manufacturers are not security pros
# [[Networked Devices#SCADA / ICS]]
# RTOS (Real-Time Operating System)
### An OS with a deterministic processing schedule
- not time to wait for other processes
- industrial equipment, automobiles
- military env
### Extremely sensitive to security issues
- non-trivial systems
- need to always be available
- difficult to know what type of security is in place
# Embedded systems
### Hardware and software designed for a specific function
- or to operate as part of a large system
### Is built with only this task in mind
- can be optimized for size and or cost
### Common examples
- traffic light controllers
- digital watches
- medical imaging systems
# High availability
### Redundancy doesn't always mean always available
- may need to be powered on manually
### HA (high availability)
- always on, always available
### May include many different components working together
- active/active can provide scalable advantages
### Higher availability almost always means higher costs
- always another contingency you could add
- upgraded power, high-quality server components, etc
