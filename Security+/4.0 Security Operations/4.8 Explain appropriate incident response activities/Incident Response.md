# Security incidents
### User clicks an email attachment and executes a malware
- malware then communicates with external servers
### DDoS
- botnet attack
### Confidential info is stolen
- thief wants money or it goes public
### User installs P2P software and allows external access to internal servers
# [[Plans and Procedures#NIST SP800-61|NIST SP800-61]]
# Preparing for an incident
### Communication methods
- phones and contact info
### Incident handling hardware and software
- laptops, removable media, forensic software, digital cameras, etc
### Incident analysis resources
- documentation, network diagrams, baselines, critical file hash values
### Incident mitigation software
- clean OS and app images
### Policies needed for incident handling
- everyone knows what to do
# The challenge of detection
### Many different detection sources
- diff levels of detail, diff levels of preparation
### Large amount of "volume"
- attacks are incoming all the time
- how do you ID the legitimate threats?
### Incidents are almost always complex
- extensive knowledge needed
# Analysis
### An incident might occur in the future
- this is your heads-up
### Web server log
- vuln scanner in use
### Exploit announcement
- Monthly Microsoft patch release, Adobe PDF software update
### Direct threats
- a hacking group doesn't like you
### An attack is underway
- or an exploit is successful
### Buffer overflow attempt
- IDed by an IDS/IPS
### Anti-virus software IDs malware
- deletes from OS and notifs admin
### Host-based monitor detects a config change
- constantly monitors system files
### Network traffic flows deviate from the norm
- requires constant monitoring
# Isolation and containment
### Generally a bad idea to let things run their course
- an incident can spread quickly
- it's your fault at that point
### Sandboxes
- an isolated OS
- run malware and analyze the results
- clean out the sandbox when done
### Isolation can be sometimes problematic
- malware or infection can monitor connectivity
- when connectivity is lost, everything could be deleted/encrypted/damaged
# Recovery
### Get things back to normal
- remove the bad, keep the good
### Eradicate the bug
- remove malware
- disable breached user accounts
- fix vuln
### Recover the system
- restore from backups
- rebuild from scratch
- replace compromised files
- tighten down the perimeter
# Lessons learned
### Learn and improve
- no system is perfect
### Post-incident meeting
- invite everyone affected by the incident
### Don't wait too long
- memories fade over time
- some recommendations can be applied to the next event
# Answer the tough questions
### What happened, exactly?
- timestamp of the events
### How did you incident plans work?
- did the process operate successfully?
### What would you do differently next time?
- retrospective views provide context
### Which indicators would you watch next time?
- diff precursors may give you better alerts
# Training for an incident
### There's limited on-the-job training when a security event occurs
- be ready when an incident is IDed
### Train the team prior to an incident
- initial response
- investigation plans
- incident reporting
- and more
### This can be an expensive endeavor
- esp. with larger response teams