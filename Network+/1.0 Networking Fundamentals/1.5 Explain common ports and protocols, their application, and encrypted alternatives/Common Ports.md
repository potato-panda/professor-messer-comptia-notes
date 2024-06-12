# Telnet - Telecommunication Network
- tcp/23
### Login to devices remotely
### Console access
### In-the-clear communication (no encryption)
### No the best choice for production systems

# SSH - Secure Shell
- Encrypted communication link tcp/22
- Looks and acts like Telnet
# DNS - Domain Name System
### Converts names to IP address - udp/53
- large transfer may use tcp/53
### These are very critical resources
- usually multiple DNS servers are in production
# SMTP (Simple Mail Transfer Protocol)
- server-to server email transfer
- ==tcp/25 (SMTP in plaintext)==
- ==tcp/587 (SMTP with encryption)==
### Also used to send mail from device to mail server
- commonly configured on mobile devices and email
### Other protocols are used for clients to receive email
- IMAP, POP3
# POP/IMAP
### Receive emails from email server
- authenticate and transfer
### POP 3 - Post office Protocol version 3
- ==tcp/110 (plaintext), tcp/995 (POP3 over TLS)==
- basic email transfer functionality
### IMAP4 - Internet Message Access Protocol v4
- ==tcp/143 (plaintext), tcp/993 (IMAP over TLS)==
- includes management of email inbox from multiple clients
# SFTP - Secure FTP
### Uses the SSH File Transfer Protocol
- ==tcp/22==
### Provides file system functionality
- resuming interrupted transfer, directory listing, remote file removal
### Encrypted communication
- uses SSH (port 22)
# File transfer appaliation protocol
### FTP - File Transfer Protocol
- ==tcp/20 (active mode data), tcp/21 (control)==
- transfer files between systems
- authenticates with a  user name and password
- full-featured functionality (list, add, delete, etc)
### TFTP - Trivial File Transfer Protocol
- ==udp/69==
- very simple file transfer protocol
	- read files and writes files
- no authentication
	- not used on production systems
# DHCP - Dynamic Host configuration Protocol
### Automated configuration of IP address, subnet mask and other options
- udp/67, udp/68
- requires a DHCP server
	- server , appliance, integrated into a SOGO router, etc
### Dynamic /pooled
- IP addresses are assigned in real-time from a pool
- each system is given a lease and must renew at set intervals
### DHCP reservation
- addresses are assigned by MAC address in the DHCP server
- quickly manage addresses from one location
# HTTP and HTTPS
### Hypertext Transfer Protocol
- communication in the browser
- any by other applications
### In the clear or encrypted
- SSL (Secure Sockets Layer) or TLS (Transport Layer Security)
![[Pasted image 20240508145146.png]]
# SNMP - Simple Network Management Protocol
### gather statistics form network devices
- ==udp/161==
### v1 - the original
- structured tables
- in-the-clear
### v2 - a good step ahead
- data type enhancements
- bulk transfers
- still in the clear
### v3 - a secure standard
- message integrity
- authentication
- encryption
### SNMP traps
- alerts and notifications from the network devices
- ==udp/162==
# Syslog
### Standard for message logging
- diverse system, consolidated log
- ==udp/514==
### Usually a central log collector
- integrated into the SIEM
### Significant storage space demand
- data storage from many devices over an extended timeframe
# RDP - Remote Desktop Protocol
### Share a desktop from a remote location over ==tcp/3389==
### Remove Desktop Services in many Windows versions
### Can connect to an entire desktop or just an application
### Clients for Windows, MacOS, Linux, Unix, iPhone and others
# NTP - Network Time Protocol
### Switches, routers, firewalls, servers, workstations
- every device has its won clock
- udp/123
### Synchgronizing the chocks becomes critical
- log files, authentication information, outage details
### Automatic updates
- no falshing 12:00 lights
### Flexible - You control how the clocks are updates
### Very accurate
- accuracy is better than 1 ms on a local network
# SIP - Session Initiation Protocol
### Voice over IP (VoIP) signaling
- ==tcp/5060 and tcp/5061==
### Setup and manage VoIP sessions
- call, ring, hang up
### Extend voice communication
- video conferencing
- instant messaging
- file transfers
- etc
# SMB - Server Message Block
### Protocol used by Microsoft Windows
- file sharing, printer sharing
- also called CIFS (common Internet File System)
### Direct over tcp/445 (NetBIOS-less)
- direct SMB communication over TCP with the NetBIOS transport
# LDAP/LDAPS
### LDAP (Lightweight Directory Access s Protocol)
- ==tcp/389==
- store and retrieve information in a network directory
###  LDAPS (LDAP Secure)
- non-standard implementation of LDAP over SSL
- ==tcp/636==
# Databases
### Microsoft SQL Server
- MS-SQL (Microsoft Structured Query language)
- tcp/1433
### Oracle SQL \*Net
- also called Oracle Net or Net8
# MySQL free and open-source database
- ultimately acquired by Oracle
- tcp/3306
