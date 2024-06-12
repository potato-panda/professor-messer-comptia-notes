### Very specific subnetting architecture
- not used since 1993
	- but still referenced in casual conversation
### Used a s a starting point when subnetting
- standard values
![[Pasted image 20240505204425.png]]

# The construction of a subnet
### Network address
- first IP address of a subnet
- set all host bits to 0 (0 decimal)
### First usable host address
- one number higher than the network address
### Network broadcast address
- last IP address of a subnet
- set all host bits to 1 (255 decimal)
### Last usable host address
- one number lower than the broadcast address
# Subnet calculations
### IP address: 10.74.222.11
- Class A
- Subnet mask 255.0.0.0
e.g 10.74.222.11

|                                            | Network | Host        |
| ------------------------------------------ | ------- | ----------- |
|                                            | 10.     | 74.222.11   |
| Network address (Set all host bits to 0)   | 10.     | 0.0.0       |
| First host address (add one)               | 10.     | 0.0.1       |
| Broadcast address (Set all host bits to 1) | 10.     | 255.255.255 |
| Last hot address (subtract one)            | 10.     | 255.255.254 |

### IP address: 10.74.222.11
- Class B
- Subnet mask 255.255.0.0

|                                            | Network | Host    |
| ------------------------------------------ | ------- | ------- |
|                                            | 176.16. | 80.200  |
| Network address (Set all host bits to 0)   | 176.16. | 0.0     |
| First host address (add one)               | 176.16. | 0.1     |
| Broadcast address (Set all host bits to 1) | 176.16. | 255.255 |
| Last hot address (subtract one)            | 176.16. | 255.254 |
|                                            |         |         |

### IP address: 192.168.4.77
- Class B
- Subnet mask 255.255.255.0

|                                            | Network    | Host |
| ------------------------------------------ | ---------- | ---- |
|                                            | 192.168.4. | 77   |
| Network address (Set all host bits to 0)   | 192.168.4. | 0    |
| First host address (add one)               | 192.168.4. | 1    |
| Broadcast address (Set all host bits to 1) | 192.168.4. | 255  |
| Last hot address (subtract one)            | 192.168.4. | 254  |
|                                            |            |      |

