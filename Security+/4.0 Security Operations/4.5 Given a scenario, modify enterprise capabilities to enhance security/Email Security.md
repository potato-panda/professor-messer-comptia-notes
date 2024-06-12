# Email security challenges
### The protocols used to transfer emails include relatively few security checks
- very easy to spoof
### Spoofing happens all the time
- check spam folder
### The email looks as if the sender is real
- but did it? how can you tell?
### A reputable sender will configure email validation
- publicly available on the sender's DNS server
# Mail gateway
### The gatekeeper
- evals the sources of inbound email
- blocks before reaching user
- on-site or cloud-based
![[Pasted image 20240610152107.png]]
# Sender Policy Framework (SPF)
### SPF protocol
- sender configs a list of all servers authz to send email for a domain
### List of authz mail servers are added to a DNS TXT record
- receiving mail servers perform a check to see if incoming email came from authz host
![[Pasted image 20240610152217.png]]
![[Pasted image 20240610152225.png]]
# Domain Key Identified Mail (DKIM)
### A mail server digitally signs all outgoing mail
- the pub key is in the DKIM TXT record
### The sig is validated by the receiving mail servers
- not user observable
![[Pasted image 20240610152334.png]]
![[Pasted image 20240610152343.png]]
# DMARC
### Domain-based Message Authentication, Reporting, and Conformance
- extension of SPF and DKIM
### Domain owner decides what receiving email servers should do with emails not validating using SPF and DKIM
- that policy is written into a DNS TXT record
- accept all, send to spam, or reject the email
### Compliance reports are sent to email admin
- the domain owner can see how emails are received
![[Pasted image 20240610152543.png]]