
### ![[Pasted image 20240506221353.png]]
### Your DNS will become very important

# IPv6 address compression
### Groups of zeros can be abbreviated with a double colon
- only one of these abbreviations allowed per address
### Leading zeros are optional
![[Pasted image 20240506221813.png]]

![[Pasted image 20240506221922.png]]

# Configuring IPv6 with a modified EUI-64
### Static addressing can be useful
- the IP address never changes
### What other address never changes? The MAC address

### Extended Unique Identifier (64-bit)
### Combined a 64-bit IPv6 prefix and the MAC address
- But wait! The MAC address is only 48-bits long
### You will need some extra bits
- and a minor change to the MAC address
# The MAC address
### Ethernet Media Access Control address
- the physical adddres of a network adapter
### EUI-48 address
- Extended Unique Identifier (48-bit)

![[Pasted image 20240506222213.png]]
# Converting EUI-48 to EUI-64
### Split the MAC
- two 3 byte (24-bit) halves
### Put FFFE in the middle
- the missing 16 bits
### Invert the seventh bit
- changed the address from the globally unique/universal
- turns the burned-in address (BIA) into a locally administered address
- This is the U/L bit (universal/local)

# Modifying the MAC

![[Pasted image 20240506222727.png]]

# Building the IPv6 address
### the 64-bit IPv6 subnet prefix
### The EUI-64 address

![[Pasted image 20240506222915.png]]

# Flipping the 7th bit
### Quickly convert the MAC address
- create a chart
### Count from 0 to F in hex
- two columns, groups of four
### Quickly convert the second character of the first hex byte
- change it to the other value
![[Pasted image 20240506223048.png]]
# Quick conversions

![[Pasted image 20240506224329.png]]

