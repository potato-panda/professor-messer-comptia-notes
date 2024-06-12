# Open permissions
### Very easy to leave a door open
- attackers will always find it
### Increasingly common with cloud storage
- statistical change of finding an open permission
### June 2017 - 14 million Verizon records exposed
- third-part left an Amazon S3 data repository open
- researcher found the data before anyone else
### Many examples
- secure permissions
# Unsecured admin accounts
### The Linux root account
- The Windows Administrator or superuser account
### Can be a misconfiguration
- intentionally configuring an easy-to-hack password
### Disable direct login to the root account
- use the ```su``` or ```sudo``` option
### Protect accounts with root or admin access
- there should be minimal numbers
# Insecure protocol
### Some protocols aren't encrypted
- all traffic sent in the clear
- Telnet, FTP, SMTP, IMAP
### Verify with a packet capture
- view everything sent over the network
### Use the encrypted versions
- SSH, SFTP, IMAPS, etc
# Default settings
### Every app and network device has a default login
- not all of these are ever changed
### Mirai botnet
- takes advantage of default configurations
- takes over IoT devices
- 60+ default configs
- cameras, routers, doorbells, garage door openers, etc
### Mirai release as open-source software
- there's a lot more where that came from
# Open ports and services
### Services will open ports
- it's important to manage access
### Often managed with a firewall
- manage traffic flows
- allow or deny based on port number or app
### Firewall rulesets can be complex
- it's easy to make a mistake
### Always test and audit
- double and triple check