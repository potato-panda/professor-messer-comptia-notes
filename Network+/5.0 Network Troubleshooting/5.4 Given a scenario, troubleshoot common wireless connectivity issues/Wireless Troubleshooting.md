# Wireless performance
### Performance can vary
- the wireless spectrum is unforgiving
- many more variables in play
### Throughput
- the amount of data successfully transferred through the wireless network
### Speed
- that maximum bandwidth available
- is generally faster as you get closer to the antennas
### Distance
- the user needs to be relatively close to the APs
# Wireless signals
###  RSSI (Receive Signal Strength Indication)
- the strength of a received radio signal
### Measures in decibel-milliwatts (dBm)
- the number of decibels (dB) with reference to one millwatt (mW)
### Show as a negative number on a log scale
- close to zero is better
	- -50dBm is excellent
	- -70dBm is good
	- -80dBm and smaller is low
![[Pasted image 20240516152120.png]]
# Wireless survey tools
- Signal coverage
- Potential interference
- Built-in tools
- 3rd-party tools
- Spectrum analyzer
![[Pasted image 20240516152231.png]]
# Troubleshooting with RSSI
https://youtu.be/LIofZvLd_04?si=wZ0un1Ays6B5-biy&t=144
# Wireless signals
### EIRP (Effective isotropic radiated power)
- the radiated signal strength
- transmit strength + antenna gain - cable loss
### In the U.S., transmission power is regulated by the FCC (Federal Communications Commissions)
- for 2.4Ghz, maximum EIRP is +36dBm or 4W
- varies based on connections and frequencies used
### Sometimes configurable on the AP
- equipment owner is responsible for managing the EIRP
![[Pasted image 20240516152538.png]]
https://youtu.be/LIofZvLd_04?si=ouDpfyagQetTdW9k&t=250
# Omnidirectional antennas
### One of the most common
- included on most APs
### Signal is evenly distributed on all sides
- place the antennas in the middle
### Good choice for most environments
- you need coverage in all directions
### No ability to focus the signal
- a different antenna will be required
# Directional antennas
### Focus the signal
- increases distances
### Send and receive in a single direction
- focused transmission and listening
### Antenna performance is measure in dB
- double power every 3dB of gain
### Yagi antenna
- very directional and high gain
### Parabolic antenna
- focus the signal to a single point
### Often used to bridge a gap
- point-to-point
- antennas are placed at both ends
# Antenna configuration
### Polarization
- the orientation of an antenna
- relative to the surface of the Earth
### Transmission and receiving polarization should be the same
- if the polarization is offset, only part of the signal will be received
![[Pasted image 20240516152951.png]]
# AP association time
### Devices must associate with an AP
- this can occur multiple times as a device roams
### Signal strength
- association is delayed or blocked due to poor signal
### Wired network controller issue
- latency and firmware issues can affect association time
### Track association metrics
- gather from the management console or via SNMP
# Channel utilization
### There's a limited amount of frequency
- everyone can't talk at one time
- similar to a wired network
### An increasing number of wireless devices
- they all want to talk
### Most APs can monitor utilization
- percentage of available air-time
- when you hit 100%, you've used up all of your available wireless space
# Managing channel utilization
### Disable legacy, low speed support
- use the fastest possible speeds and configuration
### Check your channels
- avoid overlap between AP
### Adjust the output power
- avoid conflicts with other APs
- interference can steal valuable network time
### Split the network
- you might need additional frequencies and access points
# [[Network Documentation#Site surveys|Site surveys]]