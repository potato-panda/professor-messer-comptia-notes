# ping
### Test reachability
- determine round-trip time
- uses ICMP (Internet Control Message Protocol)
### One of your primary troubleshooting tools
- can you ping the host?
https://youtu.be/6t9C72BXQHw?si=MUliVP9sxCHSn41J&t=33
# ipconfig /ifconfig / ip
### Most of your troubleshooting starts with your IP address
- ping you local router/gateway
### Determine TCP/IP and network adapter information
- and some additional IP detail
### ipconfig - Windows TCP/IP config; ifconfig - Linux interface configuration; ip address - the latest Linux utility
https://youtu.be/6t9C72BXQHw?si=l140Dwe1gjYW-Mje&t=156
# nslookup and dig
### Lookup information from DNS servers
- canonical names, IP addresses, cache timers, etc
### nslookup
- Both Windows and POSIX-based
- lookup names and IP addresses
- deprecated (use dig instead)
### dig (Domain Information Groper)
- more advanced domain information
- probably your first choice
- Windows: https://www.isc.org/downloads/bind/
https://youtu.be/6t9C72BXQHw?si=jYoMo3fwMtgtqmql&t=247
# traceroute
### Determine the route a packet takes to a destination
- map the entire path
- tracert (Windows) or tracerouter (Unix/Linux/macOS)
### Takes advantage of ICMP to Live Exceeded error message
- the time in TTL refers to hops, not seconds or minutes
- TTL=1 is the first router, TTL2 - is the second router ..
### Not all devices will reply with ICMP Time Exceeded messages
- some firewalls filter ICMP
- ICMP is low-priority for many devices
# Flavours of traceroute
### Not all traceroutes are the same
- minor differences in the transmitted payload
### Windows commonly sends ICMP echo requests
- receives ICMP time exceeded messages
- and an ICMP echo reply from the final/destination device
- unfortunately, outgoing ICMP is commonly filtered
### Some OS allow you to specify the protocol used
- Linux, Unix, MacOS, etc ...
# The mechanics of traceroute
https://youtu.be/6t9C72BXQHw?si=AhpJIbeyepxkYMH4&t=395
# Address Resolution Protocol (ARP)
### Determine a MAC address based on an IP address
- you need the hardware address to communicate
### arp - a
- view local ARP table
https://youtu.be/6t9C72BXQHw?si=W9-iWTenjS-fZCFS&t=629
# netstat
### Network statistics
- many different OSs
### netstat -a
- show all active connections
### netstat -b 
- show binaries (Windows) (show executables that are using traffic)
### netstat -n
- do not resolve names (see only IP addresses)
https://youtu.be/6t9C72BXQHw?si=iyT49S8a_DZx19Au&t=718
# hostname
### View the FQDN and IP address of the device
- very useful when there are 10 different terminal screen tabs in use
# Many different OS
- it's easy to get turned around, regardless of the OS
https://youtu.be/6t9C72BXQHw?si=E4ifQ8Wo5Hb3P8Jy&t=819
# route
### View the device's routing table
- find out which way the packets will go
### Windows: route print
### Linux, macOS, Windows: netstat -r
https://youtu.be/6t9C72BXQHw?si=d89TdNnUk_m0SO9d&t=859
# Telnet
### Telecommunication Network
- tcp/23
### Login to devices remotely
- console access
### In-the-clear communication
- avoid using in production (use SSH for console)
### A great utility for checking a port or application
- telnet 10.0.10.1 443
https://youtu.be/6t9C72BXQHw?si=J2Rd495E2COvO-vw&t=939
# tcpdump
### Capture packets from the command line
- very convenient
### Available in most OS
- included with MacOS, WinDump for Windows
### Apply filters, view in real-time
- quickly identify traffic patterns
### Save the data, use in another application
- written in standard pcap format
### Can be an overwhelming amount of data
- takes a bit of practice to parse and filter
https://youtu.be/6t9C72BXQHw?si=DR3YcKX7xah5DxFs&t=1031
# Nmap
### Network mapper
- find and learn more about network devices
### Port scan
- find devices and identify open ports
### Operating system scan
- discover the OS without logging in to a device
### Service scan
- what service is available on a device? Name, version, details
### Additional scripts
- Nmap Scripting Engine (NSE) - extend capabilities, vulnerability scans
https://youtu.be/6t9C72BXQHw?si=3oPxJaqYfnpkJjPO&t=1116
# Basic platform commands
### There are some commands that are common across switch and router manufacturers
- once you know one, you effectively know them all
### show interface
- view the interfaces on the device
- view detailed interface information
### show config
- view the device config / "show run" (in Cisco devices)
### show route
- view the routing table / "show ip route" (in Cisco devices)
![[Pasted image 20240516151508.png]]