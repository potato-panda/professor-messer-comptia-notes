# [[High Availability]]
# Server clustering
### Combine two or more servers
- appears and operates as a single large server
- users only see one device
### Easily increase capacity and availability
- add more servers to cluster
### Usually configures in OS
- all devices in cluster commonly use the same OS
![[Pasted image 20240607164448.png]]
# Load balancing
### Load is distributed across multiple servers
- servers are unaware of each other
### Distribute the load across multiple devices
- can be different OS
### Load balancer adds or removes devices
- add server to increase capacity
- remove servers not responding
# [[Recovery Sites|Site resiliency]]
# Geographic dispersion
### These sites should be physically different than the org's primary location
- many disruptions can affect a large area
- hurricane, tornado, floods, etc
### Can be a logistical challenge
- transporting equipment
- getting employee's on-site
- getting back to main office
# Platform diversity
### Every OS contain potential security issues
- you can't avoid these
### Many security vulns are specific to a single OS
- Windows vulns don't commonly affect Linux or macOS
- and vice verse
### Use many different platforms
- different apps, clients, and OSes
- spread the risk around
# Multi-cloud systems
### There are many cloud providers
- AWS, Azure, GCP, etc
### Plan for cloud outages
- can happen
### Data is both geographically dispersed and cloud server dispered
- a breach with one provider would not affect the others
- plan for every contingency
# Continuity of operations planning (COOP)
### Not everything goes according to plan
- disasters can cause a disruption to the norm
### We rely on our computer systems
- technology is pervasive
### There needs to be an alternative
- manual transactions
- paper receipts
- phone calls for transaction approvals
### These must be documented and test before a problem occurs