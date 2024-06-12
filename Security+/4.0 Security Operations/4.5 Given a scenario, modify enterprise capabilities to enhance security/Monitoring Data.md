# FIM (File Integrity Monitoring)
### Some files change all the time
- some files should NEVER change
### Monitor important OS and app files
- ID when changes occur
### Windows - SFC (System File Checker)
### Linux - Tripwire
### Many host-based IPS options
# [[Security Tools#Security Policies Data Loss Prevention (DLP) Data Loss Prevention (DLP)|Data Loss Prevention (DLP)]]
# DLP systems
### On your computer
- data in use
- endpoint DLP
### On your network
- data in motion
### On your server
- data at rest
# USB blocking
### DLP on a workstation
- allow or deny certain tasks
### November 2008 - U.S. Department of Defense
- worm virus "agent.btz" replicates using USB storage
- bans removeable flash media and storage devices
### All devices had to be updated
- local DLP agent handled USB blocking
### Ban was lifted in February 2010
- replaced with strict guidelines
# Cloud-based DLP
### Located between users and Internet
- watch every byte of network traffic
- no hardware/software
### Block custom defined data strings
- unique data for your org
### Manage access to URLs
- prevent file transfers to cloud storage
### Block viruses and malware
- anything traversing the network
# DLP and email
### Email continues to be the most critical risk vector
- inbound threats, outbound data loss
### Check every email in/outbound
- internal system or cloud-based
### Inbound
- block keywords, ID impostors, quarantine email messages
### Outbound
- fake wire transfers, W-2 transmissions, employee info
# Emailing a spreadsheet template
### November 2016
### Boeing employee emails spouse a spreadsheet to use as a template
### Contained the personal info of 36,000 Boeing employees
- in hidden columns
- SSN, DoB, etc
### Boeing sells its own DLP software
- but only uses it for classified work