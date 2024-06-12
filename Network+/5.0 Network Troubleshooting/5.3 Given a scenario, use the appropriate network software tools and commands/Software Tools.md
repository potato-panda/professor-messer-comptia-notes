# Wireless packet analysis
### Wireless networks are incredibly easy to monitor
- everyone "hears" everything
### You have to be quiet
- you can't hear the network if you're busy transmitting
### Some network drivers won't capture wireless information
- you'll need specialized adapters/chipsets and drivers
### View wireless-specific information
- signal-to-noise ratio, channel information, etc
### Try it yourself!
- https://www.wireshark.org
# Protocol analyzers
### Solve complex application issues
- get into the details
### Gathers frames on the network
- or in the air
- sometimes built into the device
### View traffic patterns
- identify unknown traffic
- verify packet filtering and security controls
### Large scale storage
# Speed test sites
### Bandwidth testing
- transfer a file, measure the throughput
### Provide useful pre- and post- change analysis
- test, install firewall/packet shaper, test again
### Measure at different times of the day
- can be automated or manual
### Not all sites are the same
- number of servers (point of presence - POP)
- bandwidth at the POP
- testing methodology
### ISP sites
- speedtest.xfinity.net
- www.att.com/speedtest
### SpeedOf.Me
### speedtest.net
### testmy.net
# iPerf
### Performance monitoring and speed testing
- your own speed test site
### Need two computers
- an iPerf server and client
### Support across many operating systems
- you can run tests everywhere
- many different options
# IP and Port scanners
### Active - scan for IP addresses and open ports
- and operating systems, services, etc
### Pick a range of IP addresses
- see who responds to the scan
### Visually map the network
- gather information on each device
- IP, operating system, services, etc
### Rogue system detection
- it's difficult to hide from a layer 2 ARP
### Nmap/Zenmap, Angry IP scanner
![[Pasted image 20240515182148.png]]
# NetFlow
### Gather traffic statistics from all traffic flows
- shared communications between devices
### NetFlow
- standard collection method
- many products and options
### Probe and collector
- probes watches network communication
- summary records are sent to the collector
### Usually a separate reporting app
- closely tied to the collector
![[Pasted image 20240515182547.png]]
![[Pasted image 20240515182602.png]]
# TFTP server
### TFTP (Trivial File Transfer Protocol)
- a bare minimum file transfer protocol
- perfect for initial file transfers and firmware upgrades
### Your device is the TFTP server
- the switch/firewall/router is the TFTP client
### Many options available for Windows, Linux, and macOS
- install and run
- there's not a lot of configuration
![[Pasted image 20240515182724.png]]
# Terminal emulator
### SSH (Secure Shell)
- encrypted terminal communication
- replaces Telnet (and FTP)
- provided secure terminal communication and file transfer features
### Windows Terminal
- any many other options