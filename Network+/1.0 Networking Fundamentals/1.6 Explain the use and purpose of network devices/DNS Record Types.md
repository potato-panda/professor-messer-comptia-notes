# DNS records
### Resource Records (RR)
- the database records of DNSs
### Over 30 record types
- IP addresses, certifications, host alias names, etc.
# Sample forward lookup file
![[Pasted image 20240509135750.png]]
# Start of Authority (SOA)
### Describes the DNS zone details
### Structure
- IN SOA (Internet zone, Start of Authority) with name of zone
- serial number
- refresh, retry, and expiry timeframes
- caching duration/TTL
![[Pasted image 20240509135855.png]]
# Address records (A) (AAAA)
### Defines the IP address of a host
- this is the most popular query
### A records are for IPv4 addresses
- modify the A record to change the hostname to IP address resolution
### AAAA records are for IPv6 addresses
- same DNS server, different records
![[Pasted image 20240509140025.png]]
# Canonical name records (CNAME)
### A name is an alias of another, canonical name
- one physical server, multiple servers
![[Pasted image 20240509140432.png]]
# Service records (SRV)
### Find a specific server
- where is Windows Domain Controller?
- where is instant messaging server?
- where is the VoIP server?
![[Pasted image 20240509140519.png]]
# Mail exchanger record (MX)
### Determines the host name for the mail server
- This isn't an IP address; it's a name
![[Pasted image 20240509140555.png]]
# Name server records (NS)
### List the name servers for a domain
- NS records point to the name of the server
![[Pasted image 20240509140624.png]]
# Pointer record (PTR)
### The reverse of an A or AAAA record
- added to a reverse map zone file
![[Pasted image 20240509140656.png]]
# Text records (TXT)
### Human-readable text information
- useful public information
### SPF protocol (Sender Policy Framework)
- prevent mail spoofing
- Mail servers check that incoming mail really did come from an authorized host
### DKIM (Domain Key Identified mail)
- digitally signs your outgoing mail
- validated by the mail server, not usually seen by the end user
- put your public key in the DKIM TXT record
![[Pasted image 20240509140913.png]]
# Zone transfers
### Replicate a DNS database
- primary DNS server has a primary copy of the zone information
### Synchronize to a secondary server
- provide redundancy
### Triggered by referencing the serial number
- if the serial number increases, there must have been a change
### Full zone transfers can be a security risk
- attackers can use the data as reconnaissance