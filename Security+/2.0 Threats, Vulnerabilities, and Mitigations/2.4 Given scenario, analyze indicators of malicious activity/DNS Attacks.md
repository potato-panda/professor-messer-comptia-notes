# DNS poisoning
### Modifying the DNS server
- requires some crafty hacking
### Modify the client host file
- host file takes precedent over DNS queries
### Send a fake response to a valid DNS request
- requires a redirection of the original request or the resulting response
- real-time redirection
- an on-path attack
# DNS spoofing / poisoning
![[Pasted image 20240606153323.png]]
# Domain hijacking
### Get access to the domain registration, and you have control where the traffic flows
- you don't need to touch the actual servers
- determines the DNS names and DNS IP addresses
### Many ways to get into the account
- brute force
- social engineer the password
- gain access to the email address that manages the account
- the usual things
### Saturday, October 22, 2016, 1PM
### Domain name registrations of 36 domains are changed
- Brazilian bank
- desktop , mobile domains and more
### Under hacker control for 6 hours
- attackers became the bank
### 5 million customers, $27 billion in assets
- results of the hack have not been publicly released
# URL hijacking
### Make money from you mistakes
- there's a lot of advantages on the net
### Sell the badly spelled domain to the actual owner
- sell a mistake
### Redirect to a competitor
- not as common, legal issues
### Phishing site
- looks like the real site, please login
### Infect with a drive-by download
- you've got a malware
# Types of URL hijacking
### Typosquatting / brandjacking
- take advantage of poor spelling
### Outright misspelling
### Typing error
### Different phrase
### Different TLD
# Wireless Attacks
### Wireless deauthn
- a significant wireless DoS attack
# 802.11 management frames
### 802.11 wireless includes a number of management frames
- frames that make everything work
- you never see them
### Important for the operation off 802.11 wireless
- how to find APs, manage QoS, associate/dissociate with an AP, etc
### Original wireless standards did not add protection for management frames
- sent in the clear, no auth or validation
# Protecting against deauth attacks
### IEEE has already addressed the problem
- updates included with 802.11ac
### Some of the important management frames are encrypted
- dissociate, deauth, channel switch announcements, etc
### Not everything is encrypted
- beacons, probes, authn, association
# Radio frequency (RF) jamming
### DoS
- prevent wireless comms
### Transmit interfering wireless signals
- decrease the signal-to-noise ratio at the receiving device
- receiving device can't hear the good signal
### Sometimes it's not intentional
- interfereance, not jamming
- microwave oven, fluorescent lights
### Jamming is intentional
- someone wants your network down
# Wireless jamming
### Many different types
- constant, random bits / Constant, legitimate frames
- data sent at random time - random data and legitimate frames
- reactive jamming - only when someone else tries to communicate
### Needs to be somewhere close
- difficult to be effective from a distance
### Time to go fox hunting
- you'll need the right equipment to hunt the jammer
- directional antenna, attenuator