# Using the right cable
### Speed/bandwidth
- theoretical maximum data rate
- usually measures in bits per second
- the size of the pipe
### Throughput
- amount of data transferred in a given timeframe
- usually measured in bits per second
- how much water is flowing through the pipe
### Distance
- know the maximum distance
- varies based on copper, fiber, repeaters, etc
![[Pasted image 20240515163514.png]]
# Unshielded and shielded cable (Twisted pair)
### Abbreviations
- U = Unshielded
- S = Braided shielding
- F = Foil shielding
### (Overall cable)/(individual pairs) TP
- Braided shielding around the entire cable and foil around the pairs is S/FTP
- Foil around the cable and no shielding around the pairs is F/UTP
![[Pasted image 20240515164756.png]]
# No plenum
![[Pasted image 20240515164838.png]]
# Plenum
![[Pasted image 20240515164942.png]]
# Plenum-rated cable
### Traditional cable jacket
- polyvinyl chloride (PVC)
### Fire-rated cable jacket
- fluorinated ethylene polymer (FEP) or low-smoke polyvinyl chloride (PVC)
### Plenum-rated cable may not be as flexible
- may not have the same bend radius
### Worst-case planning
- used in plenum and risers
- important concerns for any structure
# Serial console cables
### D-subminiature or D-sub
- the letter refers to the connector size (shape), the number denotes the number of pins
![[Pasted image 20240515165443.png]]
### Commonly used for RS-232
- recommended standard 232
- an industry standard since 1969
### Serial communications standards
- built for modem communication
- used for modems, printers, mice, networking
### Now used as a configuration port
# "Rollover" Cable
### Rolled cable, Cisco console cable, Yost cable
- serial cable "standard" proposed by Dave Yost
### A standard for RJ-45 to serial communications
### Used in conjunction with serial port connectors
![[Pasted image 20240515165710.png]]
# Console connection
![[Pasted image 20240515165724.png]]
# Ethernet cross-over cables
### Connect to Ethernet devices with using a switch
- use you crossover cable
### Can be a good alternative to a console connection
- you may not always have the right serial cable or connector
### Always carry a crossover cable
- or an adapter with the crossover
- ![[Pasted image 20240515165828.png]]
# Power over Ethernet (PoE)
### Power provided on an Ethernet cable
- one wire for both network and electricity
- phones, cameras, wireless access points
- useful in difficult-to-power areas
### Power provided at the switch
- built-in power - Endspans
- in-line power injector - Midspans
### Power modes
- Mode A - common-mode data pair power
- Mode B - Power on the spare pair
- 4-pair - Power on all four data pairs
# PoE, PoE+, PoE++
### PoE: IEEE 802.3af-2003
- the original PoE specification
- now part of the 802.3 standard
- 15.4 watts DC power, 350 mA max current
### PoE+: IEEE 802.3af-2009
- now also part of the 802.3 standard
- 25.5. watts DC power, 600mA max current
### PoE++: IEEE 802.3af-2018
- 51 W (Type 3), 600 mA max current
- 71.3 W (Type 4), 960 mA max current
- PoE with 10GBASE-T