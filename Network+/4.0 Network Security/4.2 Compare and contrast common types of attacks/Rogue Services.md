# Rogue DHCP server
### IP addresses assigned by a non-authorized server
- there's no inherent security in DHCP
### Client is assigned an invalid or duplicate address
- intermittent connectivity, no connectivity
### Disable rogue DHCP communication
- enable DHCP snooping on your switch
- authorized DHCP servers in Active Directory
### Disable the rogue
- renew the IP leases
# Rogue access points
### An authorized wireless access point
- may be added by an employee or an attacker
- not necessarily malicious
- a significant potential backdoor
### Very easy to plug in a wireless AP
- or enable wireless sharing in your OS
### Schedule a periodic survey
- walk around your building/campus
- use third-party tools / Wi-Fi Pineapple
### Consider using 802.1X (Network Access Control)
- you must authenticate, regardless of the connection type
# Wireless evil twins
### Looks legitimate, but actually malicious
- wireless version of phishing
### Configure an AP to look like an existing network
- same (or similar) SSID and security settings/captive portal
### Overpower the existing access points
- may not require the same physical location
### Wi-Fi hotspots (and users) are easy to fool
- and they're wide open
### You encrypt you communication, right?
- use HTTPS **and** a VPN
