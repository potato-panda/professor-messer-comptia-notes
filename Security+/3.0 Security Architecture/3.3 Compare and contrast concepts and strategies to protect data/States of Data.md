# Data at rest
### Data on a storage device
- HDD, SSD, flash drive, etc
### Encrypt the data
- whole disk encryption
- db encryption
- file- or folder-level encryption
### Apply permissions
- ACL
- only authz users can access data
# Data in transit
### Data transmitted over network
- also called data in-motion
### Not much protection as it travels
- many different switches, routers, devices
### Network-based protection
- firewall, IPS
### Provide transport encryption
- TLS
- IPsec
# Data in use
### Data is actively processing in memory
- system RAM, CPU registers and cache
### Data is almost always decrypted
- otherwise, you can't use it
### Attackers can pick the decrypted info out of RAM
- a very attractive option
### Target Corp. breach - November 2013
- 110 million credit cards
- data in-transmit encryption and data at-rest encryption
- attackers picked the credit card numbers out of the point-of-sale RAM
# Data sovereignty
- data that resides in a country is subject to the laws of that country
- legal monitoring, court orders, etc
### Laws may prohibit where data is stored
- GDPR (General Data Protection Regulation)
- data collected on EU citizen must be stored in the EU
- a complex mesh of tech and legalities
### Where is your data stored?
- your compliance laws may prohibit moving data out of country
# Geolocation
### Location details
- tracks within localized area
### Many ways to determine location
- 802.11, mobile carriers, GPS
### Can be used to manage data access
- prevent access from other countries
### Limit administrative tasks unless secure area is used
- permit enhanced access when inside building
