### Pretend to be something you aren't
- fake web server, fake DNS server, etc
### Email address spoofing
- the sending address of an email isn't really the sender
### Caller ID spoofing
- the incoming call information is completely fake
### On-path attacks
- the person in the middle of the conversation precents to be both endpoints
# ARP poisoning (IP spoofing)
See [[Study/professor-messer-comptia-notes/Network+/4.2/On-path attacks#ARP poisoning (spoofing)]]
# IP address spoofing
### Take someone else's IP address
- actual device
- pretend to be somewhere you are not
### Can be legitimate
- load balancing
- load testing
### May not be legitimate
- ARP poisoning
- DNS amplification / DDoS
### Easier to identify than MAC address spoofing
- apply rules to prevent invalid traffic, enable switch security
# MAC spoofing
### Your Ethernet device has a MAC address
- a unique burned-in address
- most drivers allow you to change this
### Changing the MAC address can be legitimate
- ISP expects a certain MAC address
- certain applications require a particular MAC address
### It might not be legitimate
- circumvent MAC-based ACLs (Access Control List)
- fake-out a wireless address filter
![[Pasted image 20240514171344.png]]
### Very difficult to detect
- how do you know it's not the original device?