# Attenuation
### Usually gradual
- signal strength diminishes over distance
- loss of signal intensity as signal moves through a medium
### Electrical signals through copper, light through fiber
- radio waves through the air
# Decibels (dB)
### Signal strength ratio measurements
- one-tenth of a bel
- capital V for Alexander Graham Bell
### Logarithmic scale
- add and subtract losses and gains
### 3bD = 2x the signal
### 10bD = 10x the signal
### 20dD = 100x the signal
### 30bD = 1000x the signal
# dB loos symptoms
### No connectiveity
- no signal!
### Intermittent connectivity
- just enough signal to sync the link
### Poor performance
- signal too weak
- CRC errors, data corruption
### Test each connection
- test distance and signal loss
# Avoiding EMI and interference
### Electromagnetic interference
### Cabling handling
- no twisting - don't pull or stretch
- watch your bend radius
- don't use staples, watch your cable ties
### EMI and interference with copper cables
- avoid power cords, fluorescent lights, electrical systems, and fire prevention components
### Test after installation
- you can find most of your problems before use
# Troubleshooting pin-outs
### Cables can foul up a perfectly good plan
- test your cables prior to implementation
### Many connectors look alike
- do you have a good cable mapping device?
### Get a good cable person
- it's an art
# Incorrect pin-out
### Near and far pins in cable aren't where they are supposed to be
- pin 1 goes to pin 1, pin 2 to pin 2 ..
### Performance or connectivity issues
- may drop from 1Gb/s to 100Mb/s
- may not connect at all
![[Pasted image 20240515171143.png]]
# Bad ports
### Interface errors
- may indicate bad cable or hardware problem
### Verify configurations
- speed, duplex, VLAN
### Verify two-way traffic
- e2e connectivity
![[Pasted image 20240515171230.png]]
# Interface configuration problems
### Poor throughput
- very consistent, very reproducible
### No connectivity
- no link light
### No connectivity
- link light and activity light
# Interface configuration
### Auto vs. Manual configuration
- personal preference
### Light status
- no light, no connection
### Speed
- must be identical on both sides
### Duplex
- if mismatched, speed with suffer
- increase in late collisions
# Open and shorts
### A short circuit
- two connections are touching
- wires inside of a cable or connection
### An open circuit
- a break in the connection
### Complete interruption
- can be intermittent
# Troubleshooting opens and shorts
### May be difficult to find
- the wire has to be moved just the right way
- wiggle it here and there
### Replace the cable with the short or open
- difficult or impossible to repair
### Advanced troubleshooting with a TDR
- Time Domain Reflectometer
# Incorrect transceivers
### Transceiver have to match the fiber
- single mode transceiver connects to single mode fiber
### Transceiver needs to match the wavelength
- 850nm, 1310nm
### Use the correct transceivers and optical fiber
- check the entire link
### Signal loss
- dropped frames, missing frames
# Transceiver mismatch
![[Pasted image 20240515171937.png]]
# Duplex/speed mismatch
### Speed and duplex
- speed: 10/100/1000/Auto
- duplex: half/full/Auto
### Incorrect speed
- many switch configurations will auto-negotiate speed
- less than expected throughput
### Incorrect duplex
- again, the switch may auto-negotiate
- needs to match on both sides
- a mismatch will cause significant slowdowns
- increase in late collisions may indicate a duplex mismatch
# Reversing transmit and receive
### Wiring mistake at
- cable ends
- punchdowns
### Easy to find with a wire map
- 1-3, 2-6, 3-1, 6-2
- simple to identify
### Some network interfaces will automatically correct (Auto-MDIX)
![[Pasted image 20240515172512.png]]
# TX/RX reversal troubleshooting
### No connectivity
- Auto-MDIX might connect
- try turning it on
### Locate reversal location
- often at a punchdown
- check your patch panel
![[Pasted image 20240515172801.png]]
# Dirty optical cables
### Light needs to be seen
- fiber connectors must be clean
- always use your dust caps
### Dirty connectors will inhibit or prevent communication
- attenuation can prevent data transfer
### Clean through before using
- just before installation