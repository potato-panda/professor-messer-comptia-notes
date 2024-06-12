<iframe width="560" height="315" src="https://www.youtube.com/embed/XMzLpGKTu50?si=siOEMg4ktmkjSjz8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
# Subnetting a network
![[problem 1.png]]

# We have four networks with about 40 devices per subnet
![[chart.png]]
![[subnet example.png]]

# Four important addresses
### Network address / subnet ID
- first address in the subnet
### Broadcast address
- last address in subnet
### First available host address
- one more than the network address
### Last available host address
- one less than the broadcast address

# Magic number subnetting
### Very straightforward method
- can often perform the math in your head
### Subnet with minimal math
- still some count involved
### Come charts might help
- but may not be requires
- CIDR to decimal
- host ranges

# Some helpful charts
### CIDR to decimal charts
- memorization will increase speed
![[cidr to deci.png]]

![[Pasted image 20240506165440.png]]
![[Pasted image 20240506165506.png]]
# Host ranges
- larger blocks are easier to remember
- multiply quickly for the smaller blocks
![[Pasted image 20240506165636.png]]

# The magic number process
### Convert the subnet mask to decimal (if necessary)
### Identify the "interesting octet"
### Calculate the "magic number"
- 256 minus the interesting octet
### Identify the network address
- first address in the range
### Identify the broadcast address
- last address in the range
# Find the subnet ID

### IP address: 165.245.77.14; Subnet: 255.255.240.0
### If mask is 255, copy the IP address
### If mask is 0, copy the 0
### If none of the above, it is the "interesting octet"

![[Pasted image 20240506170245.png]]

### Subtract the interesting octet mask from 256: 256 - 240 = 16
### The magic number is therefore 16
- the interesting octet range is 16
![[Pasted image 20240506170504.png]]
### Therefore the subnet ID is 165.245.64.0

# Find the broadcast address

### IP address: 165.245.77.14; Subnet mask 255.255.240.0; Subnet ID: 165.245.64.0

### If mask is 255, copy the IP address
### If mask is 0, use 255
### If none of the above, it is the "interesting octet"

### Subtract the interesting octet mask from 256
- 256 - 240 = 16
### Calculate Subnet ID + Magic Number - 1
- 64 +16 - 1 = 79
### Therefore broadcast address is 165.245.79.255

# Find the host range

### First host is subnet ID + 1
- 165.245.64.1
### Last host is broadcast address - 1
- 165.245.79.254
### All done

