# Security log files
### Details security-related info
- blocked and allows traffic flows
- exploit attempts
- blocked URL categories
- DNS sinkhole traffic
### Critical security info
- documentation of every traffic flow
- summary of attack info
- correlate with other logs
# Firewall logs
### Traffic flows through the firewall
- source/dest IP, port numbers, disposition
### NGFW
- logs the app used, URL filtering categories, anomalies and suspicious data
# Application logs
### Specific to the application
- info varies widely
### Windows
- event viewer / application log
### Linux / macOS
- /var/log
### Parse the log details in the SIEM
- filter out unneeded info
# Endpoint logs
### Attackers often gain access to endpoints
- phones, laptops, tablets, desktops, servers, etc
### Data on the endpoint
- logon events, policy changes, system events, processes, account management, directory services, etc.
### Everything rolls up to the SIEM
### Use with correlation of security events
- combine IPS events with endpoint status
# OS-specific security logs
### OS security events
- monitoring apps
- brute force, file changes
- authn details
### Find problems before they happen
- brute force attacks
- disabled services
### May require filtering
- don't forward everything
# IPS/IDS logs
### Logs contain info about predefined vulns
- known OS vulns, generic security events
### Common data points
- timestamp
- type or class of attack
- source/dest IP
- source/dest port
# Network logs
### Switches, routers, APs, VPN concentrators
- and other infra devices
### Network changes
- routing updates
- authn issues
- network security issues
# Metadata
- data that describes other data sources
### Email
- header details, sending servers, dest IP
### Mobile
- type of phone, GPS location
### Web
- OS, browser type, IP
### File
- name, address, phone number, title
# [[Study/professor-messer-comptia-notes/Network+/4.1/Risk Management#Vulnerability scan results|Vulnerability scans]]
# Automated reports
### Most SIEMs include a report generator
- automate common security reports
### May be easy or complex to create
- the SIEM may have it's own report generator
- third-party report generations may be able to access the database
### Requires human intervention
- someone has to read the reports
### These can be involved to create
- huge data storage and extensive process time
# Dashboards
### Real-time status info
- get summaries on a single screen
### Add or remove info
- most SIEMs and reporting systems allow for customization
### Shows the most important data
- not designed for long-term analysis
# Packet captures
### Solve complex application issues
- get into the details
### Gathers packets on the network
- or in the air
- sometimes built into the device
- 
### View detailed traffic info
- ID unknown traffic
- verify packet filtering and security controls
- view a plain-language description of the app data