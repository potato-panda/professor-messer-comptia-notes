# NTP (Network Time Protocol)
### Switches, routers, firewalls, servers, workstations
- every device has it's own clock
### Synchronizing the clocks becomes critical
- log files, authentication information, outage details
### Automatic updates
- not flashing 12:00 lights
### Flexible
- you control how clocks are updates
### Very accurate
- accuracy is better than 1 ms on a local network
# NTP clients and servers
### NTP server
- listens on udp/123, responds to time requests from NTP clients
- does not modify their own time
### NTP client
- requests time updates from the NTP server
### NTP client/server
- requests time updates from the NTP server
- responds to time requests from other NTP clients
### Important to plan your NTP strategy
- which devices are clients, servers, client/servers?
# NTP stratum layers
### Some clocks are better than others
- your distance from the original reference clock is a stratum
### Stratum 0
- atomic clock, GPS clock,
- very accurate
### Stratum 1
- synchronized to stratum 0 servers
- Primary time servers
### Stratum 2
- synced to stratum 1 servers
# Configuring NTP
### NTP client
- specify the NTP server address (IP or hostname)
- use multiple NTP servers (if available) for redundancy
### NTP server
- you need at least one clock source
- specify the stratum level of the clock
- if there's a choice, the lowest stratum is used
![[Pasted image 20240509143103.png]]
