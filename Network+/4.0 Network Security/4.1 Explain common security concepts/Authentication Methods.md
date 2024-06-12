# Local authentication
### Authentication credentials are stored on the local device
- must be individually administrated
### Very manual process
- a password change must be done manually on all devices
### Doesn't rely on a third-party authentication server
- a network outage won't impact the login process
# Multi-factor authentication (MFA)
### More than one factor
- something you are
- something you have
- something you know
- somewhere you go
- something you do
### Can be expensive
- separate hardware tokens
- specialized scanning equipment
### Can be inexpensive
- free smartphone applications
# RADIUS (Remote Authentication Dial-in User Service)
### One of the more common AAA protoocls
- supported on a wide variety of platforms and devices
- not just for dial-in
### Centralize authentication for users
- routers, switches, firewalls,
- server authentication
- remote VPN  access
- 802.11x network access
### RADIUS services available on almost any server operating system
# TACACS
### Terminal Access Controller Access-Control System
- remote authentication protocol
- created to control access to dial-up lines to ARPANET
### TACACS+
- latest version
- more authentication requests and response codes
- released as an open standard in 1993
# LDAP (Lightweight Directory Access Protocol)
### Protocol for reading and writing directories over an IP network
- an organized set of records, like a phone directory
### X.500 specification was written by the International Telecommunications Union (ITU)
- they know directories
### DAP ran on the OSI protocol stacks
- LDAP is lightweight
### LDAP is the protocol used to query and update an X.500 directory
- used in Windows Active Directory, Apple OpenDirectory, Novell eDirectory, etc
# Kerberos
### Network authentication protocol
- authenticate once, trusted by the system
- no need to re-authenticate to everything
- mutual authentication - the client and the server
	- protect against on-path or replay attacks
### Standard since the 1980s
- developed by MIT
### Microsoft started using Kerberos in Windows 2000
- based on Kerberos 5.0 open standard
- compatible with other operating systems and devices
# SSO with Kerberos
### Authenticate one time
- lost of backend ticketing
- cryptographic tickets
### No constant username and password input
- saves time
### Only works with Kerberos
- not everything is Kerberos-friendly
### There are many other SSO methods
- smart-cards, SMAL, etc
# Which method to use?
### Many different ways to communicate to an authentication server
- more than a simple login process
### Often determined by what is at hand
- VPN concentrator can talk to a RADIUS server
- we have a RADIUS server
### TACACS+
- probably a Cisco device
### Kerberos or LDAP
- probably a Microsoft network
# IEEE 802.1X
- Port-based Network Access Control (NAC)
- you don't get access to the network until you authenticate
### EAP integrates with 802.1X
- Extensible authentication protocol
- 802.1X prevents access to the network until the authentication succeeds
### Used in conjunction with an auth database
- RADIUS, LDAP, TACACS+, Kerberos, etc
# EAP
### Extensible Authentication Protocol
- an authentication protocol/framework
### Many different ways to authenticate based on RFC standards
- manufacturers can build their own EAP methods
### EAP integrates with 802.1X
- prevent access to the network until the authentication succeeds