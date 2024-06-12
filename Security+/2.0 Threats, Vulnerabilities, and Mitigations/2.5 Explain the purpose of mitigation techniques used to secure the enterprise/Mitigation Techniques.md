# Patching
### Incredibly important
- system stability, security fixes
### Monthly updates
- incremental (and important)
### Third-party updates
- app devs, device drivers
### Auto-update
- not always the best option
### Emergency out-of-band updates
# Encryption
### Prevent access to app data files
- file system encryption
### File level encryption
- Windows Encrypting File System (EFS)
### Full disk encryption (FDE)
- encrypt everything on the drive
- BitLocker, FileVault, etc.
### Application data encryption
- managed by the app
- stored data is protected
# Monitoring
### Aggregate information from device
- built-in sensors, separate devices
- integrated into servers, switches, routers, firewalls, etc.
### Sensors
- IPS, firewall logs, auth logs, web server access logs, db transaction logs, email logs
### Collectors
- proprietary console (IPS, firewall), SIEM consoles, syslog servers
- many SIEMs include a correlation engine to compare diverse sensor data
# Least privilege
### Rights and permission should be set to the bare minimum
- you only get exactly what's needed to complete your objective
### All user accounts must be limited
- apps should run with minimal prvileges
### Don't allow users to run with admin privileges
- limits the scope of malicious behaviour
# Configuration enforcement
### Perform a posture assessment
- each time a device connects
### Extensive check
- OS patch version
- EDR (Endpoint Detection and Response) version
- status of firewall and EDR
- certificate status
### Systems out of compliance are quarantined
- private VLAN with limited access
- recheck after making corrections
# Decommissioning
### Should be a formal policy
- don't throw your data into the trash
- someone can find it later
### Mostly associated with storage devices
- hard drive
- SSD
- USB drives
### Many options for physical devices
- recycle the device for use in another system
- destroy the device