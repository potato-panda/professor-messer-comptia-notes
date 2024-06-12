# The subnet mask
### Contiguous series of series
- ones on the left
- zeroes on the right
![[The subnet mask.png]]

| network = 24 bits  | host = 8 bits     |
| ------------------ | ----------------- |
| 11111111.11111111. | 11111111.00000000 |
| 8 + 8 + 0 +        | 0                 |
| /24                |                   |
# Binary to CIDR-block notation (slash notation after the IP address e.g. 192.168.1.0/24)

Count the ones from the left side (16 ones = /16)

| network = 16 bits  | host = 16 bits    |
| ------------------ | ----------------- |
| 11111111.11111111. | 00000000.00000000 |
| 8 + 8 +            | 0 . 0             |
| /16                |                   | 

| network = 26 bits             | host = 6 bits |
| ----------------------------- | ------------- |
| 11111111.11111111.11111111.11 | 000000        |
| 8 + 8 + 8 + 2                 |               |
| /26                           |               |

| network = 12 bits | host = 20 bits         |
| ----------------- | ---------------------- |
| 11111111.1111     | 0000.00000000.00000000 |
| 8 +    4 +        | 0 + 0                  |
| /12               |                        | 

# Subnet masks - binary to decimal
![[Subnet masks - binary to decimal reference chart.png]]
![[Subnet masks - binary to decimal example.png]]
![[Subnet masks - binary to decimal example 2.png]]

# CIDR-block notation to decimal
![[Pasted image 20240506154249.png]]
![[Pasted image 20240506160634.png]]
