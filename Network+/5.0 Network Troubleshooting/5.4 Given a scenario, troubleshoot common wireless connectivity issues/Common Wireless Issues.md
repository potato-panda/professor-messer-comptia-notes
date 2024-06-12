# Overlapping channels
![[Pasted image 20240516153723.png]]
https://youtu.be/zyo5Iv6v3uU?si=ph2i_jZRaSiQZU7J
# Attenuation
### Wireless signals get weaker as you move further from the antenna
- the attenuation can be measured with a Wi-Fi analyzer
### Control the power output on the AP
- not always an option
### Use a receive antenna with a higher gain
- capture more of a signal
### Some power is lost in the antenna cable coax
- most applicable at higher frequencies
- also check for damaged cables, especially outside
# Wrong SSID
### Every AP has at least one Service Set Identifier (SSID)
- but did you connect to the right one?
### This can be more confusing than you think
- public Wi-Fi Internet
- Guest internet
- internet
### Confirm the correct SSID settings
- should be listed in the current connection status
# Wrong passphrase
### Wireless authentication
- many different methods
### Required to connect to the wireless network
- if not connected, check the authentication
### Shared passphrase
- common in a SOHO, not in the enterprise
### 802.1X
- used for the enterprise
- make sure the client is configured to use 802.1X
# Security type mismatch
### Encryption on wireless is important
- make sure the client matches the AP
### This is much easier these days
- almost everything is at the level of WPA2/3
### Some legacy equipment may not be able to keep up
- if you change the AP, you may not be able to support it
### Migrate all of your WEP to WPA2/3
- and any WPA
# Incorrect antenna placement
### Interference
- overlapping channels
### Slow throughput
- data fighting to be heard through the interference
### Check AP locations and channel settings
- a challenge for 2.4Ghz
- much easier for 5Ghz
# Wireless coverage
![[Pasted image 20240516155145.png]]
# Captive portal
### Authentication to a network
- common on wireless networks
### Access table recognizes a lack of authentication
- redirects your web access to a captive portal page
- use a username/password to authenticate
### Authentication timeout
- may require re-authenticate after an interval
### Portal is probably authenticating to an external database
- check the back-end RADIUS/LDAP/TACACS process
# Client disassociation
### A denial of service attack
- takes advantage of older 802.11 management frame transmission
### Device keeps dropping from the wireless network
- or never connects
### Disassociation frames can be clearly seen in a packet capture
- grab the 802.11 frame information with Wireshark
### Remove the device performing the disassociation
- or upgrade to a new 802.11 standard