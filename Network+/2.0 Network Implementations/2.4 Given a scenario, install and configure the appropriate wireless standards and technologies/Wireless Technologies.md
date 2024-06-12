# 802.11 technologies
### Frequency
- 2.4GHz or 5 GHz
- sometimes both
- and sometimes additional bands
### Channels
- groups of frequencies, numbers by the IEEE
- using non-overlapping channels would be optimal
### Bandwidth
- amount of frequency in use
- 20, 40, 80, 160 MHz
# Band selection and bandwidth
![[Pasted image 20240513140429.png]]
# 802.11 channel bandwidths and bonding
### 802.11a/b/g (20/22/20MHz)
### 802.11n (20/40/80MHz)
- increase bandwidth with bonded channels
- In 2.4GHz, a 40 MHz channel uses over 80% of the available bandwidth
### 802.11ac (20/40/80/80+80/160MHz)
- 40MHz for 802.11n stations, 80MHz required for 802.11ac stations
- 160MHz optional (contiguous or non-contiguous bonded channels)
### 802.11ax (20/40/80/80+80/160MHz)
- similar bandwidths to 802.11ac
# Independent basic service set (IBSS)
### Two devices communicate directly to each other using 802.11
- no AP required
### Ad hoc
- Created for a particular purpose without any previous planning
- without an AP
### Temporary or long-term communication
- connect to a device with an ad hoc connection
- configure it with the AP settings and credentials
# SSID and BSSID
### Every wireless network needs a name
- SSID (Service Set Identifier)
### There might be multi AP supporting an SSID
- how does your computer tell them apart?
- the hardware address of an AP is a BSSID (Basic Service Set Identifier)
- the MAC (Media Access Control) address
![[Pasted image 20240513141918.png]]
# Extending the network
### Most organizations have more than one AP
- tens or hundreds
### Wireless network names can be used across AP
- makes it easier to roam from one part of the network to another
### The network name shared across AP is an ESSID
- extended Service Set Identifier
### Your device automatically roams when moving between AP
- you don't have to manually reconnect
# ESSID
![[Pasted image 20240513142147.png]]
# Counting antennas
### Net technologies were added to 802.11n , 802.11ac, 802.11ax
- send multiple streams of information over the same frequency at the same time
- 802.11n - MIMO (Multiple-Input and Multi-Ouput)
- 802.11ac - Downstream MU-MIMO (Multi-user MIMO)
- 802.11ax - Downstream and Upstream MU-MIMO
### Number of antennas (802.11n/ac/ax)
- used to determine the number of available streams
- (antennas on the AP) x (antennas on the client): number of streams
- 2x2:2, 3x3:2, 4x4:4
# Before 802.11n
![[Pasted image 20240513142901.png]]
# MIMO
![[Pasted image 20240513143719.png]]
# MU-MIMO
![[Pasted image 20240513143820.png]]
# 802.11ax MU-MIMO
![[Pasted image 20240513143847.png]]
# 802.11ax MU-MIMO with OFDMA
![[Pasted image 20240513143927.png]]
# Omni-directional antennas
### One of the most common
- included on most AP
### Signal is evenly distributed on all sides
- omni-all
### Good-choice for most environments
- you need coverage in all directions
### No ability to focus the signal
- a different antenna will be required
![[Pasted image 20240513144624.png]]
# Directional antennas
### Focus the signal
- increased distances
### Send and receive in a single direction
- focused transmission and listening
### Antenna performance is measured in dB
- double power every 3dB of gain
![[Pasted image 20240513144609.png]]
### Yagi antenna
- very directional and high gain
### Parabolic antenna
- focus the signal to a single point
![[Pasted image 20240513144556.png]]
