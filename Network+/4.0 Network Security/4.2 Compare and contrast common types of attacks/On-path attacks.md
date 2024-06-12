# On-path network attack
### How can an attacker watch without you knowing?
- formerly known as man-in-the-middle
### Redirects your traffic
- then passes it on to the destination
- you never know your traffic was redirected
### ARP poisoning
- on-path attack on the local IP subnet
- because ARP has no security
# ARP poisoning (spoofing)
![[Pasted image 20240514154124.png]]
![[Pasted image 20240514154130.png]]
![[Pasted image 20240514154149.png]]
![[Pasted image 20240514154203.png]]
![[Pasted image 20240514154242.png]]
![[Pasted image 20240514154252.png]]
![[Pasted image 20240514154319.png]]
# DNS poisoning
### Modify the DNS server
- requires some crafty hacking
### Modify the client host file
- the host file takes precedent over DNS queries
### Send a fake response to a valid DNS request
- requires a destination of the original request or the resulting response
- real-time redirection
- this is an on-path attack
# DNS spoofing / poisoning
![[Pasted image 20240514154535.png]]
![[Pasted image 20240514154604.png]]
![[Pasted image 20240514154629.png]]
![[Pasted image 20240514154849.png]]
# Other on-path attacks
### Get in the middle of the conversation and view or change information
- session hijacking
- HTTP spoofing
- Wi-Fi eavesdropping
### Encryption fixes most of these situations
- you can't change what you can't see