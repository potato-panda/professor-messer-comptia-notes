### Put the change mgnt process into action
- execute plan
### There's not such thing as a simple upgrade
- can have many moving parts
- separate events may be required
### Change mgnt is often concerned with "what" needs to change
- the technical team is concerned with "how" to change it
# Allow list / deny list
### Any app can be dangerous
- vulns, trojan horses, malware
### Security policies can control app execution
- allow list, deny/block list
### Allow list
- nothing runs unless approved
- very restrictive
### Deny list
- nothing on the "bad lest" can be run
- anti-virus, anti-malware
# Restricted activities
### The scope of change is important
- defines exactly which components are covered
### A change approval isn't permission to make any change
- the change control approval is very specific
### The scope may need to be expanded during the change window
- impossible to prepare for all possible outcomes
### The change mgnt process determines the next steps
- there are processes in place to make the change successful
# Downtime
### Services will eventually be unavailable
- the change process can be disruptive
- usually scheduled during non-prod hours
### If possible, prevent any downtime
- switch to secondary system, upgrade primary then switch back
### Minimize any downtime events
- process should be as automated as possible
- switch back to secondary if issues appear
- should be part of the backout plan
### Send emails and calendar updates
# Restarts
### It's common to require a restart
- impl the new config
- reboot OS, power cycle the switch, bounce the service
- can the system recover from power outage?
### Services
- stop and restart the service or daemon
- may take seconds or minutes
### Apps
- close the app entirely
- launch a new app instance
# Legacy apps
### Some apps were here before you arrived
- they'll be here when you leave
### Often no longer supported by the devs
- you're now the support team
### Fear of the unknown
- face your fears and document the system
- it may not be as bad as you think
### May be quirky
- create specific processes and procedures
### Become the expert
# Dependencies
### To complete A, must complete B
- a service will not start w/o other active services
- an app requires a specific library version
### Modifying one component may require changing or restarting other components
- this can be challenging to manage
### Dependencies may occur across systems
- upgrade the firewall code first
- then upgrade the firewall mgnt software
# Documentation
### Can be challenging to keep up with changes
- documentation can be outdated quickly
- require with change mgnt process
### Updating diagrams
- modifications to network config
- address updates
### Updating policies/procedures
- adding new systems may require new procedures
# Version control
### Track changes to a file or config data over time
- easily revert to a previous setting
### Many opportunities to manage versions
- router configs
- Windows OS patches
- app registry entries
### Not always straightforward
- some devices and OS provide version control features
- many require additional mgnt software