# MAC filtering
### Media Access Control
- the "hardware" address
### Limit access through the physical hardware address
- keeps the neighbors out
- additional administration with visitors
### Easy to find working MAC addresses
- MAC addresses can be spoofed
- free open-source software
### Security through obscurity
- if you know the method, you can easily defeat it
# Antenna placement
### Focus coverage to the necessary work areas
- limit access from outside the building
### Adjust power levels
- control coverage based on signal strength
### May require some additional site surveys
- walk around and optimize coverage
![[Pasted image 20240514190459.png]]
![[Pasted image 20240514190447.png]]
![[Pasted image 20240514190557.png]]
> 2.4GHz has channels 1, 6, 11 placed where they don't overlap to maximize coverage and minimize interference
# Wireless isolation
### Wireless client isolation
- wireless devices on an AP can't communicate with each other
- useful in hotel or public area
- may not be useful at work with P2P applications
### Guest network isolation
- guest network does not have access to the internal private network
- this is almost always the right configuration
# Wireless security modes
### Configure the authentication on your wireless AP / wireless router
### Open System
- no authentication password is required
### WPA/2/3-Personal / WPA/2/3-PSK
- WPA2/3 with a pre-shared key
- everyone sues the same 256-bit key
### WPA/2/3-Enterprise / WPA/2/3-802.1X
- authenticates users individually with an authentication server (i.e. RADIUS)
![[Pasted image 20240514191034.png]]
# EAP
### Extensible Authentication Protocol)
- an authentication protocol
### Many different ways to authenticate based on RFC standards
- WPA 2/3 uses five EAP types as authentication mechanisms
### Some version of EAP is used when authenticating to the network
- common to integrate on wireless networks using 802.1X
# Geofencing
### Some MDMs allow for geofencing
- restrict or allow features when the device is in a particular area
### Cameras
- the camera might only work when outside the office
### Authentication
- only allow logins when the devices is located in a particular area
# Captive portal
### Authentication to a network
- common on wireless networks
### Access table recognizes a lack of authentication
- redirects your web access to a captive portal page
### Username/password
- and additional authentication factors
### Once proper authentication is provided, the web session continues
- until the captive portal removes your access
![[Pasted image 20240514191540.png]]
# IoT security
### Internet of Things devices
- smart devices, appliances, garage doors, door locks, lights, etc
### Security is probably not the primary focus
- in some cases, it's not a consideration at all
### IoT devices should be segmented from the private network
- keep you personal devices and storage systems away from IoT devices
- if IoT device is breaches, your personal data is not accessible
### Use a separate VLAN
- many home AP provide a "guest" network
- this is different than the DMZ or screened-subnet